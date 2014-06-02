---
layout: post
title:  "Sincronizar pasta via ssh"
date:   2014-06-01 21:19:49
categories: jekyll update
---

****
comando para sincronizar um computador via ssh:

	rsync -ravzup [diretório] [user]@[machine]:[diretório]

flags:

* -r de cópia recursiva
* -a de modo de arquivamento
* -v de modo verbose, para mostrar na tela tudo o que ele está fazendo
* -z para compactar o arquivo durante a transferência (e descompactar no destino)
* -u modo update. Se o arquivo não foi atualizado, pula para o próximo, poupando tempo.
* -p preserva as permissões dos arquivos