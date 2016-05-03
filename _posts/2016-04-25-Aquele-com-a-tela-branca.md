---
published: true
title: A Tela Branca d̶a̶ ̶M̶o̶r̶t̶e̶ do Ionic
layout: post
---
<center>
<img src="https://www.firebase.com/resources/images/blog/ionic-blank-template.png" width="25%" title="Tela branca erro Ionic" alt="Tela branca do ionic">
</center>

A tela toda em branco no Ionic acontece, por causa do Content Security Policy(CSP), presente na nova versão do Cordova 5x que alterou algumas politicas de seguranças, basicamente ele controla solicitações de rede, imagens, src e etc, através do webview.

Como o Ionic utiliza AngularJS e por sua vez angular utiliza o modelo MVC, que utiliza o src para montar suas rotas, para contornar o problema é bem simples, é só colocar uma meta tag no seu index, entre as tags do head:

```<meta http-equiv="Content-Security-Policy"content="default-src *; style-src 'self' 'unsafe-inline'; script-src 'self' 'unsafe-inline' 'unsafe-eval'">```

Essa meta tag permite acesso total, existem outras, com menos acesso, você pode conferir no Cordova Whitelist, que tem toda a documentação bonitinha.

Caso o problema da tela em branco continue, pode ser por causa da versão do android e então seria necessário add o[crowssalk](https://ionickers.github.io/2016/04/23/aquele-sobre-crosswalk.html).

<center>
Assine o Canal no Telegram!<br>
<a href="https://telegram.me/ionickers">
<img src="http://sempreupdate.org/wp-content/uploads/2016/03/telegram-icon-hdcast.png" width="35%">
</a>
</center>


Links
===

[Cordova Whitelisting](https://github.com/apache/cordova-plugin-whitelist)

[Cordova Whitelist](http://docs.ionic.io/docs/cordova-whitelist)