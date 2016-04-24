---
published: true
title: Aquele sobre Crosswalk
layout: post
---
<center>
<img src="https://crosswalk-project.org/assets/identity/crosswalkproject-logo-horizontal-dark.png" width="85%" title="Aquele sobre Crosswalk" alt="Crosswalk Project">
</center>

<br><br>

Mas que p☠rr@ é o Crosswalk?
===

O Crosswalk é um wrapper do projeto Chromium para Android, contando com as mesmas características do navegador, criando uma webview com mais compatibilidade com as aplicacoes, os dispositivos Android com versoes 4X e inferior sao equipados com webview diferente do mantido pelo Google, muitas veses nao recebendo atualizacoes das fabricantes, e com pouco compatibilidade com os recursos atuais, diferente da versao 5X e superior, que tem o webview é mantido pelo Google, como um aplicativo separado recebendo atualizacoes diretamente da Google Play.

Apesar de se basear no Chromium para Android, o Crosswalk possui alguns diferenciais próprios:

* Não é mostrada a barra de endereços e abas, pois o projeto funciona em tela cheia, como se fosse um aplicativo nativo. Então, não é preciso usar a ação Request fullscreen do objeto Browser.
* No Chrome para Android, uma música só pode ser iniciada com um evento de toque. Já no Crosswalk a música pode ser tocada a qualquer momento.
* No Crosswalk é possível usar as condições On back button, On menu button e On search button do objeto Browser (funcionam apenas no projeto exportado). No navegador estas condições não funcionam.

Para instalar o Crosswalk na sua aplicacao é bem simples, apenas instale o plugin

```$ cordova plugin add cordova-plugin-crosswalk-webview
```
ou

```$ ionic browser add crosswalk
```
Voce tambem pode adcionar o plugin de forma mais facil ainda, se voce estiver usando o intelXDK, basta dar um check no input.

<img src="https://ionickers.github.io/public/images/crosswalk.png">


[Project Crosswalk](https://crosswalk-project.org)

[IntelXDK](https://software.intel.com/pt-br/intel-xdk)