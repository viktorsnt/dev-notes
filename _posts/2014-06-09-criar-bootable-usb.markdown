---
layout: post
title: "Criando um usb bootable para instalar mavericks"
date: 2014-06-09 14:24:40
categories: terminal usb macosx mavericks
---

## usando createinstallmedia

No Mavericks existe um programa em Unix escondido nele chamado createinstallmedia. (isso aí, tem que usar o Terminal).

*obs: funciona apenas no Lion, Mountain Lion ou Mavericks.*

1. Formate um pendrive de 8GB para Mac OS Extended com o nome *Untitled*
2. use o comando `sudo /Applications/Install\ OS\ X Mavericks.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ OS\ X\ Mavericks.app --nointeraction`
3. Este comando vai apagar todo conteúdo do pendrive, e vai pedir sua senha de admin
4. Espere terminar. Vai demorar uns 20/30 minutos