# git-cheat

 compilador de markdown para HTML estático
=======================================

Este projeto é um gerador de websites estáticos com as seguintes características:

* Simplicidade e facilidade de uso.
* Baseado em arquivos de texto com formatação básica.
* Pouca dependência em aplicações e bibliotecas externas.
* Fácil de hospedar em qualquer local.
* O conteúdo pode ser convertido noutros formatos.

Apostila:
https://docs.google.com/document/d/1vA8ZdYBTj3ptqwK0JAxS2ydfmwVqSu9Lsh0Q_nbQCUo/edit?usp=sharing

Slides:
https://drive.google.com/open?id=1Zjfonb6N7jQIeO-WUXOLdUUMpn0RRu3L3790XHFqoHY

Dependências
------------

Utilize o script `pandocToHTML-dependencies` para fazer a instalação das dependências num
ambiente de hospedagem compatível com o Debian GNU/Linux.

No windows baixe o arquivo compactado (zip) do pandoc em: https://github.com/jgm/pandoc/releases/tag/2.3.1
e descompacte na pasta pandoc-2.3

Criando um site
---------------

Vamos ilustrar com simples comandos:

    # Crie a pasta do seu site já com a pasta de dados
    mkdir -p ~/projetos/blog/data

    # Entre na pasta
    cd ~/projetos/blog

    # Crie uma página inicial
    echo "Oi mundo!" > data/index.md

    # Compile!
    sh pandocToHTML

O sítio compilado será criado na pasta `output`, pronta para ser
copiada para um ambiente web.

Mantendo o blog pelo git
------------------------

    # Inicialize
    git init

    # Ignore o site compilado do versionamento
    git ignore output

    # Adicione o resto
    git add .

    # Cometa as mudanças iniciais
    git commit -m "Versão inicial"

Documentação adicional e exemplo
--------------------------------

Um arquivo de exemplo contendo a documentação básica se encontra
na pasta `data` e pode ser gerada pelo próprio projeto!
