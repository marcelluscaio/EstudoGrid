Fazer somente grid:
1 - Display 
2 - Flex  x Grid
3 - Exemplos com grid



Grid:

1) Criando o grid
grid-template-columns
grid-template- rows
Vendo no devtools

Grid container x grid item x grid cell

Grid explicito x grid implicito
- Voce cria os grids, mas o grid cria grids implicitos

com px
Com %
com fr
  - fr eh espaco livre. MOstrar i que acontece quando tem um conteudo com width grande demais e com conteudo maior que os outros
com auto
% + fr (Nunca use % somando 100%)

minmax()



Repeat


2) Posicionando no grid 

- grid-column / grid-row
  - span 2, 3 (o que acontece se nao houver mais colunas? pula par aa linha debaixo)
  - span maior qur o grid explicito (ma pratica!)
  - 1/3
  - 2 / 5 x span 2 / 5, 2 / span 2
  - 1 / -1 (Nao sabe o tamanho? Do inicio ao final)
  - span 2 / -1 (As duas ultimas)
  - O que acontece com -1 se voce nao define grids explicitos?

- grid-template-areas + grid-area

- Order (isso pode baguncar a ordem que o leitore de tela lê, e a seleção do conteúdo com mouse)





3) Gap
 - cuidado com %


4) Alinhamento
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


5) Ainda criando o grid: auto fill e auto fit (geralmente queremos esse)


6) grid-auto flow dense
(quando um fica mmuito grande, o grid deixa espaco em branco. essa propriedade resolve isso)



Referencias:

https://cssgrid.io/

https://css-tricks.com/snippets/css/complete-guide-grid/


