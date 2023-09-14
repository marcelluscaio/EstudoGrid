# Introdução a CSS GRID
</br>

## Roteiro
</br>

### Criando o grid
</br>

- Usando o devtools
- grid-template-columns e grid-template- rows
  - Com px
  - Com %
  - Gap (cuidado com %)
  - Com fr
    - fr precisa de espaço livre Mostrar:
      - Conteúdo com width grande demais
      - Conteudo maior que os outros
  - Com auto
  - % + fr (Nunca use % somando 100%)

- Grid container x grid row x grid column x grid cell x grid item
- Grid explicito x grid implicito
- Repeat
- minmax()
- auto fill e auto fit
- fit-content()
- Hierarquia
  - Tamanho do elemento pai >= tamanho do grid >= Tamanho das colunas + (gap * (numero de colunas -1))
  - Coluna >= Elemento

</br>

### Posicionando elementos no grid 
</br>

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

</br>

### Alinhando o grid e os items do Grid
</br>

- Justify-content, align-content, place-content
  - Lida com as celulas em relacao ao grid. Precisa de espaço no grid
  - Valores: stretch, start, end, center, space-around, space evenly, space between;
  - Padrão stretch se a largura das colunas ou altura das linhas não é definida. Se for definida, passar a ser start.

- Justify-items, align-items, place-items
  - Lida com o conteudo dentro das células. Precisa de espaço na célula;
  - Valores: stretch, start, end, center;
  - Padrão stretch se a largura ou altura do elemento não são definidas. Se forem definidas, passar a ser start.

- Justify-self, align-self, place-self
  - Similar à família dos -items, é usado direto no elemento. Lida com o conteudo dentro da célula. Precisa de espaço na célula;
  - Valores: stretch, start, end, center;
  - Padrão stretch se a largura ou altura do elemento não são definidas. Se forem definidas, passar a ser start.

</br>

### Estudos de caso
</br>

Exercicios
https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grid_skills

Exercicio da Alura
https://codepen.io/marcelluscaio/pen/zYyvWvb

EM CONSTRUCAO

</br>

## Referências:
</br>

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
