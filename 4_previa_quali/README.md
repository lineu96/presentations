# MEPC · Métodos Estatísticos em Pesquisa Científica

## Instruções para os autores

O diretórios e arquivos são usados da seguinte forma:

  1. `config/`: onde são mantidos os arquivos de configuração dos
     slides.
     1. `preamble-global.tex`: dão as configurações globais de estilo
        Beamer.
     2. `preamble-commands.tex`: estão definidos comandos e ambientes.
     3. `preamble-author.tex`: define informações dos autores e
        instituição.
     4. `preamble-chunk-rnw.tex`: define ambientes relacionados à codigo
        R.
     5. `preamble-refs.tex`: define opções relacionadas às referências
        bibliográficas.
     6. `dest-texto-2.png`, `ufpr-transparent-600px.png` e
        `ufpr-fundo-16x9.jpg`: são logos e imagem de fundo.
     7. `setup.R`: define opções globais dos chunks.
  2. `pics/`, `Rfigs/` e `figure/`: onde são arquivadas as imagens
     usadas nos slides.
  3. `refs.bib`: armazena as referências bibográficas em BibTeX.

Para ver os pacotes R que são usados, execute o arquivo
`./used_R_packages.sh` e veja o conteúdo criado no arquivo `DEPENDS`.

```sh
sh used_R_packages.sh
cat DEPENDS
```

Para renderizar cada `Rnw`, execute o arquivo `render_each.sh`.

```sh
sh render_each.sh
```

## Repositórias de imagens

Imagens a serem usadas nos slides, preferencialmente, devem ser
retiradas de repositórios de imagens na Web. Deve ser citado a fonte das
imagens em todas as legendas de figuras para não sejam violados direitos
de uso. Os sites geralmente indicam como fazer a citação apropriada da
fonte das imagens.

  1. https://www.pexels.com/pt-br/
  2. https://pixabay.com/pt/images/
  3. https://unsplash.com/s/photos/
  4. https://www.freeimages.com/
  5. https://www.kindpng.com/
  6. https://github.com/walmes/Tikz

**Atenção**: quando a imagem apresentar várias resoluções disponíveis,
escolher aquela mais próxima do intervalo 600 a 800px. Isso é para
economia de espaço em disco e também porque imagens acima dessa
resolução não farão diferença nos slides.
