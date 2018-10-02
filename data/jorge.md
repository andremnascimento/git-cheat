Git-Cheat: gerador de websites estáticos
========================================
uygugugyguy

Implementação
-------------

O projeto é um script escrito em bash que utiliza o [Pandoc](http://pandoc.org)
para compilar um website completo a partir de arquivos de texto usando a formatação
Markdown.

Desenvolvimento
---------------

Para gerar o conteudo em Markdown você pode utilizar os seguinte editores online:

    * [StackEdit](https://stackedit.io/app)
    * [Editor.md](https://pandao.github.io/editor.md/en.html)

Fazendo um release
------------------

    # Comece o desenvolvimento configurando o git-flow
    git flow init

    # Sempre desenvolva a partir do branch develop
    git checkout develop

    # Faça um release conforme o necessário
    git flow release init VERSAO

    # etc!

