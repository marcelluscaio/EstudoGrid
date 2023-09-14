# Introdução a CSS GRID

## Roteiro

### Criando o grid
grid-template-columns
grid-template- rows
Vendo no devtools

Grid container x grid item x grid cell

Grid explicito x grid implicito
- Voce cria os grids, mas o grid cria grids implicitos

com px
Com %

Gap
 - cuidado com %

com fr
  - fr eh espaco livre. MOstrar i que acontece quando tem um conteudo com width grande demais e com conteudo maior que os outros
com auto
% + fr (Nunca use % somando 100%)

Repeat

minmax()

Ainda criando o grid: auto fill e auto fit (geralmente queremos esse)


Deixar claro:
Hierarquia:
Tamanho do elemento pai >= tamanho do grid >= Tamanho das colunas + (gap * (numero de colunas -1))
Coluna >= Elemento


### Posicionando elementos no grid 

- grid-column / grid-row
  - span 2, 3 (o que acontece se nao houver mais colunas? pula par aa linha debaixo)
  - span maior qur o grid explicito (ma pratica!)
  - 1/3
  - 2 / 5 x span 2 / 5, 2 / span 2
  - 1 / -1 (Nao sabe o tamanho? Do inicio ao final)
  - span 2 / -1 (As duas ultimas)
  - O que acontece com -1 se voce nao define grids explicitos?

grid-auto flow dense
(quando um fica mmuito grande, o grid deixa espaco em branco. essa propriedade resolve isso)

- grid-template-areas + grid-area

- Order (isso pode baguncar a ordem que o leitore de tela lê, e a seleção do conteúdo com mouse)





### Alinhando o grid e os items do Grid
Lida com as celulas em relacao ao grid. Precisa de espaço no grid
justify-content (Padrao start. end, center, space-around, space evenly, space between )
align-content (Padrao start. end, center, space-around, space evenly, space between )
place content


Lida com o conteudo dentro das células
Justify-items (padrao stretch. Valores start, center, end)
align-items (padrao stretch. Valores start, center, end)
place items (cuidado com a comaptibilidade)

Usado direto na celula
justify-self
align-self



### Estudos de caso
Exercicios
https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grid_skills

Exercicio da Alura
https://codepen.io/marcelluscaio/pen/zYyvWvb

EM CONSTRUCAO


## Referências:

Curso WesBos
https://cssgrid.io/

Grid CheatSheet
https://css-tricks.com/snippets/css/complete-guide-grid/


KEVIN POWELL
Get started with grid WITHOUT being overwhelmed
https://www.youtube.com/watch?v=8QSqwbSztnA

Learn CSS Grid the easy way
https://www.youtube.com/watch?v=rg7Fvvl3taU

Easier layouts with these 3 Grid tips
https://www.youtube.com/watch?v=z2kuC7w9emE

Auto fill x auto fit
https://css-tricks.com/auto-sizing-columns-css-grid-auto-fill-vs-auto-fit/

Fit content
https://developer.mozilla.org/en-US/docs/Web/CSS/fit-content_function

KEVIN POWELL
The magic of auto-fit and auto-fill (and the difference between them)
https://www.youtube.com/watch?v=qjJR3qYCd54

LAYOUT LAND
https://www.youtube.com/watch?v=tFKrK4eAiUQ
