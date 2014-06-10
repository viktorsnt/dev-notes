---
layout: post
title: "Hospedar um blog Ghost no GitHub Pages"
date: 2014-06-10 19:23:20
categories: ghost github
---

O GitHub Pages apenas aceita sites estáticos, então para podermos instalar um blog Ghost, precisamos de uma gambiarra:

1. instale buster: `pip install buster`, buster precisa do *wget*, então: `brew install wget`
2. Inicie Ghost localmente e carregue seu tema, crie seus artigos, e faça as mudanças que você quer
3. Agora crie um repositório no <a href="http://github.com/new/" target="_blank">GitHub</a>
4. Crie um diretório para gerar os arquivos estáticos e configure o buster: `buster setup` e entre o endereço do repositório que seria: http://github.com/*username*/*repositório*
5. Após configurar, rode: `buster generate --domain=http://localhost:2368`, será criada uma pasta chamada *static*
6. `cd static`, e dê um push `git add --all` e depois `git commit -m "seu commit"`, e `git push origin gh-pages`
7. Se quiser deletar a branch master do github: `git push origin :master`