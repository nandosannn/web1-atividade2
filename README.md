# Atividade II

#### Seletores

Tipo de Seletor | Sintaxe | Descrição | Exemplo
:--------------| :------- | :--------- | :--------
Seletor de Tipo | `elemento` | Aplica estilos a todos os elementos de um tipo específico (tag HTML). | `p { color: blue; }`
Seletor de Classe | `.classe `| Aplica estilos a elementos com uma classe específica. | `.container { margin: 20px; }`
Seletor de ID | `#id` | Estiliza o elemento com um ID específico. | `#header { background-color: gray; }`
Seletor Universal | `* `| Aplica estilos a todos os elementos da página. | `* { margin: 0; padding: 0; }`
Seletor de Atributo | `[atributo]` |	Aplica estilos a elementos que possuem um determinado atributo. |	`input[type="text"] { width: 200px; }`
Seletor Descendente	| `elemento1 elemento2` |	Seleciona elementos que são descendentes de um elemento específico. |	`div p { color: red; }`
Seletor de Filho Direto |	`elemento1 > elemento2` | Seleciona elementos que são filhos diretos de um elemento. |	`ul > li { list-style: none; }`
Seletor de Irmão Adjacente |	`elemento1 + elemento2` |	Seleciona o elemento imediatamente após um elemento especificado. |	`h1 + p { margin-top: 0; }`
Seletor de Irmãos Gerais |	`elemento1 ~ elemento2`|	Seleciona todos os elementos irmãos de um tipo específico, após o primeiro elemento. |	`h1 ~ p { color: gray; }`
Pseudo-classe Dinâmica |	`:pseudo-classe` |	Seleciona elementos com base em estados dinâmicos, como hover, focus, active.	| `button:hover { background-color: blue; }`
Pseudo-classe Estrutural | `:pseudo-classe` |	Seleciona elementos com base em sua posição estrutural, como first-child, nth-child. |	`li:nth-child(2) { color: green; }`
Pseudo-elemento | `::before	elemento::before` |	Insere conteúdo antes do conteúdo real de um elemento. |	`p::before { content: "Nota: "; }`
Pseudo-elemento | ::after	elemento::after | 	Insere conteúdo depois do conteúdo real de um elemento. |	`p::after { content: "Fim"; }`
Pseudo-elemento |  `::first-line	elemento::first-line` | Estiliza a primeira linha do conteúdo de um elemento. |	`p::first-line { font-weight: bold; }`
Pseudo-elemento | `::first-letter	elemento::first-letter` | 	Estiliza a primeira letra do conteúdo de um elemento. |	`p::first-letter { font-size: 2em;`

<br>

#### Prioridade

Prioridade | Tipo de Seletor | Exemplo | Pontuação
:-------- | :-------------- | :------- | :--------
1 |	Estilo Inline |	`<p style="color: red;">` |	1000
2 |	ID	#header | `{ color: blue; }` |	100
3 |	Classe, Atributo e Pseudo-classe |	`.container { color: green; } `|	10
4	| Tipo (Tag) |	`p { color: black; }` |	1
5 |	Seletor Universal |	`* { color: gray; }` | 0

<br>

#### Box Model

Box Model é um conceito para descrever como elementos html são estruturas em uma página como, por exemplo, o espaçamento interno e externo.

Propriedade | Descrição |	Exemplo
:-------- | :---------- | :----------
`content` |	Área onde o conteúdo do elemento é exibido (texto, imagem, etc.). É definida por width e height. |	`width: 200px; height: 100px;`
`padding` |	Espaço interno entre o conteúdo e a borda do elemento. Aumenta a área de fundo sem afetar a borda. |	`padding: 10px;`
border |	Define a borda ao redor do padding e do conteúdo. Inclui propriedades como estilo, largura e cor. |	`border: 2px solid black;`
margin | 	Espaço externo ao redor da borda do elemento, separando-o dos outros elementos. |	`margin: 15px;`

<br>

#### Unidades de Tamanho

Unidade | Descrição | Exemplo
:------- | :-------- | :-------
px | Unidade de tamanho em pixel, usado para definir tamanhos fixos de tela. | `20px`
pt | Unidade fixa usado para impressão. | `20pt` 
em | Unidade definida com base no tamanho do elemento pai no HTML, usado para criar layout de tamanhos variáveis. | Se o font-size do pai for `16px`, então font-size: `2em`; no elemento filho será `32px`.
rem | Unidade definida com base no tamanho do elemento raiz do HTML `<html>`, que por padrão é `16px`. | `2rem` é `32px`
