# Resumo HTML e CSS

Este documento apresenta um conteúdo resumido sobre os principais conceitos de HTML e CSS.

## HTML

### O que é?

HTML (HyperText Markup Language) é a linguagem de marcação fundamental para a criação de páginas web. Define a estrutura e o significado do conteúdo da página, permitindo a organização e apresentação de texto, imagens, vídeos, entre outros elementos. Em outras palavras, HTML é o esqueleto de uma página web.

### Estrutura Básica

A estrutura básica de um documento HTML é composta por três elementos principais: html, head e body. A tag html compõe todo o arquivo HTML, inclusive todas as outras tags e é essencial para criação de um arquivo em HTML. A tag (head) contém informações sobre o documento como o título da página, enquanto a tag (body) contém o conteúdo visível da página, como textos, imagens e links. Dentro da tag (head), é necessário colocar a tag (title) que define o título da página web.

### Tags e Atribuições

As tags HTML são como as etiquetas que marcam o início e o fim de um elemento dentro de uma página web. Elas indicam ao navegador como o conteúdo deve ser exibido, como títulos, parágrafos, imagens, links, etc. Além disso, existem as atribuições das tags que são informações adicionais nas quais fornecem contexto e funcionalidades a um elemento HTML. São pares de nome/valor que aparecem dentro da tag de abertura e influenciam a sua apresentação ou comportamento. 

Por exemplo a tag (img) onde contém src que diz a fonte da imagem deve-se colocar entre aspas o link da imagem ou nomedaimagem.extensão, logo isso é um atributo da tag. Entretanto, esse atributo é obrigatório na tag imagem, mas existem atributos que são opcionais como dar um tamanho a imagem como atributo width ="100". Veja agora as principais tags utilizadas em um arquivo HTML:

```sh
---------------------------- Principais Tags ----------------------------

<!DOCTYPE html> ---> Use versão HTML5, não é tag 
<html> </html> ---> Arquivo HTML
<head> </head> ---> Cabeça do Arquivo
<body> </body> ---> Corpo do Arquivo
<title> </title> ---> Título do Documento
<meta charset="UTF-8"> ---> Evita erros de Acentuação
<meta name="viewport" content="width=device-width, initial-scale=1.0"> ---> Responsividade
<link href="caminho" rel="stylesheet"> ---> Linkar com Arquivo CSS
<style> </style> ---> Estilização CSS

---------------------------- Tags Estruturais ----------------------------

<div class="curso"> </div> ---> Container genérico para agrupar elementos e não tem peso semântico. Geralmente vem junto com atributo class usado para aplicar estilos CSS.
<span> </span> ---> Similar a div só que não ocupa uma linha inteira, fica dentro da linha. Não tem peso semântico.
<nav> </nav> ---> Container que geralmente define uma área de navegação. Menus, links para outras páginas e barra de navegação do site.
<aside> </aside> ---> Container que geralmente define conteúdo lateral ou secundário. barras lateraisanúncios, links complementares e conteúdos relacionados.
<section> </section> ---> Container que geralmente define uma seção temática da página. Pode conter títulos, parágrafos e artigos
<article> </article> ---> Container que apresenta conteúdo independente e completo, que faz sentido sozinho. Comentários e textos.
<figure> ---> Container que apresenta conteúdo ilustrativo como por exemplos as imagens.
  <figcaption> </figcaption> --> Legenda da imagem
</figure> ---> Container que apresenta conteúdo ilustrativo como por exemplos as imagens.
<header> </header> ---> Container que serve para cabeçalho de página, pode conter nav por exemplo.
<main> </main> ---> Container mostra o contéudo principal da página. Só pode existir um main.
<footer> </footer> ---> Containter que serve de rodapé da página. Contatos, direitos autorais, créditos.

---------------------------- Formatação de Texto ----------------------------

<h1> </h1> ---> Cabeçalho Um
<p> </p> ---> Parágrafo
<br> ---> Pula Linha
<hr> ---> Cria linha Divisão
<strong> </strong> ---> Negrito Semântico
<small> </small> ---> Pequeno
<i> </i> ---> Itálico
<! -- --> ---> Comentário
<blockquote> </blockquote> ---> Citação Longa

---------------------------- Elementos de Mídia ----------------------------

<a href="URL">Nome</a> --> Link
<img src="caminho" alt="descrição (acessibilidade)" width="largura" height="altura"> ---> Imagem
<video src="caminho" width="largura" controls(adiciona controles:play, pause, volume)></video>
<audio src"caminho" controls(adiciona controles:play, pause, volume)></audio>
<iframe src="URL" width="largura"> </iframe> ---> Página dentro de outra Página

---------------------------- Listas Ordenadas e Não Ordenadas ----------------------------

<ol> ---> Lista Ordenada
  <li> </li> --> Item da Lista
  <li> </li> --> Item da Lista
</ol> ---> Lista Ordenada
<ul> ---> Lista Não Ordenada
  <li> </li> --> Item da Lista
  <li> </li> --> Item da Lista
</ul> ---> Lista Não Ordenada

---------------------------- Tabelas ----------------------------

<table> ---> Tabela
  <caption> </caption> ---> Título da Tabela
  <tr> --> Linha da Tabela
    <th> Nome </th> --> Cabeçalho
    <th> Curso </th> --> Cabeçalho
    <th> Nota </th> --> Cabeçalho
  </tr> --> Linha da Tabela
  <tr> --> Linha da Tabela
    <td> Artur </td> --> Célula de dados da Linha
    <td> ADS </td> --> Célula de dados da Linha
    <td> 8 </td> --> Célula de dados da Linha
  </tr> --> Linha da Tabela
</table> ---> Tabela

---------------------------- Formulários ----------------------------

<form action="onde os dados serão enviados" method="get(dados aparecem na URL — ideal para buscas) ou post(dados ocultos — ideal para login, cadastro, envio seguro)"> ---> Formulário
  <label> </label> --> Rótulo do Campo
  <input type="text, email, password, number, date, time, checkbox (opções múltiplas), radio (uma opção entre várias), file (envia arquivos), submit (envia tipo botão) ou reset (limpar)"    name="nome do campo" placeholder="texto de dica dentro do campo"> --> Campo de entrada
  <label for="msg">Mensagem:</label> --> "for" associa o o rótulo com o input e no input estará o mesmo valor no "id"
  <textarea id="msg" name="mensagem"></textarea> --> Campo de entrada grande
  <select name="curso"> --> Lista de Seleção
    <option value="eh-o-que-na-verdade-vai-mandar-para-o-back-end-em-vez-de-HTML-eh-esse-texto">HTML</option> --> Opção da Lista
    <option value="css">CSS</option> --> Opção da Lista
    <option value="js">JavaScript</option> --> Opção da Lista
  </select> --> Lista de Seleção 
  <button type="submit">Enviar</button> --> Botão (se difere do input type submit por ser mais flexível)
</form> ---> Formulário
```

## CSS

### O que é?

CSS (Cascading Style Sheets) é a linguagem de estilo usada para descrever a apresentação visual de um documento escrito em linguagens como HTML, controlando seu design, layout, cores, fontes e espaçamento.

### Propriedades e valores

Uma propriedade é uma característica de um elemento do HTML (cor de fundo, largura, altura, espaçamento, etc). Um valor define o resultado de uma propriedade e como o navegador deve exibir o estilo daquele elemento. Um exemplo disso é: background (propriedade): red (valor);

### Formas de Declaração CSS

CSS Inline: Adiciona o código CSS utilizando o atributo style dentro das tags HTML, tag por tag. 
Vantagens: Fácil e rápido para testes; Afeta somente aquele elemento; Não precisa de arquivo CSS separado.
Desvantagens: Difícil manutenção; Não pode ser reaproveitado; Utilizado para alterações muito específicas e únicas, como sobrescrever um estilo visto que o CSS Inline tem prioridade em cima das outras forma de declaração.

CSS Interno: Adiciona o código CSS dentro da tag (head) da página HTML. Dentro dessa tag, é adicionado a tag (style) e colocamos as regras de CSS nessa área. 
Vantagens: Código centralizado no próprio arquivo HTML; Mais organizado que inline. Permite reaproveitar estilos na mesma página.
Desvantagens: Não reaproveita estilos entre várias páginas; Arquivo HTML fica grande.

CSS Externo: Cria um arquivo CSS com todas as regras CSS que queremos aplicar e esse arquivo é referenciado no HTML da página através da tag (link). 
Vantagens: Melhor organização e manutenção; Reutilização de estilos em várias páginas; HTML fica limpo.
Desvantagens: Depende de requisição extra (pode afetar carregamento mínimo em internet lenta); Não funciona offline se a importação falhar.

```sh
--- CSS Inline ---

<p style="color: red; font-size: 20px;">Texto</p>

--- CSS Interno ---

<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>

--- CSS Externo ---

<link rel="stylesheet" href="caminho"> ---> colocar no head da página HTML, atributo rel indica relação entre o arquivo atual com o arquivo CSS nesse caso

-- dentro do arquivo css
p {
      color: blue;
    }
```

### Seletores

Seletores CSS são padrões que o navegador usa para encontrar e aplicar estilos a elementos HTML específicos. <br> Veja alguns tipos de seletores e combinadores que existem:

```sh
--- Seletor por Tipo/Tag: Busca elementos por uma tag HTML ---

p {
      background: blue;
    }

--- Seletor por ID: Busca elementos através do atributo id ---

#texto {
      color: red;
    }

<p id="texto"> Olá </p> 

--- Seletor por Classe: Busca elementos através do atributo class ---

.texto {
    background: green;
}

<p class="texto"> Olá </p> 

--- Seletor Universal: Seleciona todos os elementos do HTML ---

* {
  font-weight: bold;
}

--- Seletores de Atributo: Seleciona elementos que possuem um atributo específico e consegue também buscar atributo com um valor específco ---

[title] {
  color: blue;
} 

[title="Netflix"] {
  color: red;
}

[title~="Streaming"] {
  background: black;
} 

Obs: esse apresenta ~, ou seja, ele busca ou a palavra exata ou que pelo menos tenha essa palavra, por exemplo: "Streaming Netflix", "Prime Streaming", "Streaming", etc. Precisa ter pelo menos espaço, não pode ser "StreamingNetflix" ou "PrimeStreaming".

[title|="Streaming"] {
  background: black;
} 

Obs: esse apresenta |, ou seja, ele busca ou a palavra exata ou que pelo menos tenha essa palavra seguida de hífen, por exemplo: "Streaming-Netflix", "Streaming". Não funciona com "Prime-Streaming", pois a palavra buscada que precisa vir hífen depois dela e não antes.

[href^="http://"] {
  background: green;
}

Obs: atributo indicando que o valor que tiver esse prefixo "http://" vai receber a estilização.

[href$="com"] {
  background: blue;
}

Obs: atributo indicando que o valor que tiver esse sufixo "com" vai receber a estilização.

[href*="escola"] {
  background: yellow;
}

Obs: atributo indicando que se tiver esse valor "escola" em qualquer lugar do link, sem importar se é prefixo ou sufixo, vai receber a estilização.

--- Agrupamento de Seletores: Aplica as mesmas regras de CSS para seletores diferentes utilizando vírgula ---

.texto, h1, p, div, [title], #texto {
  color: pink;
}

.texto.teste {
  color: blue;
}

<div class="texto teste"> </div>

Obs: Aplica a estilização só para a classe "texto teste", se tiver só texto ou só teste não funciona.

p.texto {
  background: gray;
}

Obs: Esse último especifíca que para aplicar o fundo cinza precisa ser um seletor com tag p e classe .texto.

--- Combinador Descendente: Relação entre dois seletores ou mais por meio de espaços  ---

div p {
  color: purple;
}

#lista01 li {
  background: black;
}

.fundoverde #sublista01 li {
  color: red;
}

--- Combinador Filho: Relação entre dois seletores ou mais utilizando o > ---

div > p {
  background: orange;
}

--- Combinador Irmão Adjacente: Relação entre dois seletores ou mais utilizando o +, no caso do irmão é porque a tag deve estar na mesma nível de indentação e adjacente, pois ele aplicará a estilização logo no irmão em seguida ---

div + p {
  color: tomato;
}

--- Combinador Irmão em Geral: Relação entre dois seletores ou mais utilizando o ~, no caso do irmão é porque a tag deve estar na mesma nível de indentação e em geral, pois ele aplicará a estilização em todos os irmãos independentemente se estiver logo em seguida ou não ---

div ~ p {
  background: green;
}

Obs: É possível utilizar todos os conceitos de seletores, agrupamento e combinadores juntos, basta utilizar a criatividade em seus projetos!
```

### Dimensionamento e Espaçamento

Largura = width: valor; <br>
Largura Mínima = min-width: valor; <br>
Largura Máxima = max-width: valor; <br>
Altura = height: valor; <br>
Altura Mínima = min-height: valor; <br>
Altura Máxima = max-height: valor; <br>

Margem: Espaçamento por fora dos elementos (tags). Existem 5 tags de estilização de margem que são: <br>
  
  ```sh
  margin-top: valor; --> margem referente ao topo do elemento.
  margin-left: valor; --> margem referente à esquerda do elemento.
  margin-right: valor; --> margem referente à direita do elemento.
  margin-botom: valor; --> margem referente à parte abaixo do elemento.
  margin: valor; --> vai depender da quantidade de valores inseridos, por exemplo:
    margin: 10px; --> em todos os lados;
    margin: 10px 20px; --> primeiro valor: em cima e embaixo, segundo valor: lados;
    margin: 10px 20px 30px; --> primeiro valor: em cima, segundo valor: lados, terceiro valor: embaixo;
    margin: 10px 20px 30px 40px; --> primeiro valor: em cima, segundo valor: direita, terceiro valor: embaixo, quarto valor: esquerda;
  ```
Padding: Responsável por espaçar o conteúdo interno dos elementos. Por exemplo, existe uma div que possue um parágrafo colado em todos os lados, se aplicarmos o padding, é possível descolar o parágrafo, deixando uma borda interna que no caso é o padding. Segue a mesma estrutura das propriedades de margem: <br>

  ```sh
  padding-top: valor; --> margem referente ao topo do elemento.
  padding-left: valor; --> margem referente à esquerda do elemento.
  padding-right: valor; --> margem referente à direita do elemento.
  padding-botom: valor; --> margem referente à parte abaixo do elemento.
  padding: valor; --> vai depender da quantidade de valores inseridos, por exemplo:
    padding: 10px; --> em todos os lados;
    padding: 10px 20px; --> primeiro valor: em cima e embaixo, segundo valor: lados;
    padding: 10px 20px 30px; --> primeiro valor: em cima, segundo valor: lados, terceiro valor: embaixo;
    padding: 10px 20px 30px 40px; --> primeiro valor: em cima, segundo valor: direita, terceiro valor: embaixo, quarto valor: esquerda;

  Obs: Importante notar que quando aumenta o padding, pode aumentar também a altura e largura do elemento. Portanto, pode ser interessante utilizar o box-sizing!
  width = largura + borda + padding
  height = altura + borda + padding
  ```
  
Box-sizing: Responsável por calcular o tamanho total de um elemento (largura e altura). Controla se padding e border entram ou não na conta da largura/altura.

Valores: auto = define um valor automático; initial = define um valor padrão/inicial; inherit = herda valor de propriedade da tag pai, content-box = padrão do CSS, adiciona padding e border por fora, border-box = respeita a largura aplicada, já incluindo padding e border.

### Estilizações Básicas 

```sh
--- CORES ---

Pré-Definidas: Cores já estabelecidas na estilização, basta escrever o nome delas. Para saber mais, acessar o site: https://www.w3schools.com/tags/ref_colornames.asp

color: purple;
border: 2px solid currentcolor; 
// palavra currentcolor referencia a cor atual do valor atual da propriedade color, nesse caso a cor da borda será roxo.

RGB: Função rgb() que apresenta os valores de vermelho, verde e azul que podem variar de 0 a 255. Pode  utilizar também a porcentagem.

color: rgb(255,255,255); ---> branco
background: rgb(100%,0%,0%); --> vermelho

RGBA: Função rgba() é similar ao rgb() e apresenta transparência da cor. Esse último valor varia de 0.0 (máximo de transparência) até 1.0 (sem nível de transparência).

color: rgba(255,255,255,0.0); 
background: rgba(0,0,0,1.0); 

Hexadecimal: Formado por hashtag mais 6 dígitos, sendo 3 pares, um para vermelho, outro para verde e o último para azul. Variam de 00 (menor intensidade) para FF (maior intensidade). Os números variam de 0 a 9 e os caracteres variam de A a F. É possível adicionar transparência também que varia de 00 a FF.

color: #00FF00; ---> verde sem transparência
color: #00FF0000; ---> verde com transparência

HSL: Composto por Hue (matiz), Saturation (saturação) e Lightness (luminosidade). Hue varia em graus na roda de cores de 0 a 360, onde 0 ou 360 é vermelho, 120 é verde e 240 é azul. Saturation varia em porcentagem onde 0% é cinza e 100% é cor com intensidade total. Lightness também possue valor percentual onde 0% é preto e 100% é branco.

color: hsl(0,100%,30%);

HSLA: Extende do HSL, a única mudança é a transparência de cor que varia de 0.0 (máximo de transparência) até 1.0 (sem nível de transparência).

color: hsla(0,100%,30%,0);

--- IMAGENS ---

Propriedade object-fit: Determina como a imagem/vídeo vai ser redimensionada para caber na caixa do elemento. Sem precisar escrever, já vem como padrão "object-fit: fill;". Nesse caso, a imagem ou vídeo pode acabar sendo distorciada de acordo com os valores estabelecidos de largura e altura. 
Por isso, é interessante utilizar o "object-fit: contain;", pois mantém as proporções da imagem/vídeo, embora ocorra a possiblidade de não preencher todo o espaço. Um outro valor que existe é o "object-fit: cover;", no qual a imagem/vídeo cobre toda a área exigida mas acaba cortando parte da imagem/vídeo. Outra forma que pode ser é "object-fit: none;", onde mantém a proporção original, ignorando todo dimensionado estabelecido. Por último, existe o "object-fit: scale-down;" que se consiste nas configurações do contain e do none e escolhe qual dessas configurações teria uma imagem menor para se basear.

Propriedade object-position: Determina como a imagem/vídeo deve ser posicionada no elemento. Sem precisar escrever, já vem como padrão "object-position: 50% 50%";". Esses valores significam respectivamente o eixo x e o eixo y, ou seja, o 50% 50% quer dizer que a imagem está centralizada. Nesses valores é possível utilizar outras unidades de medidas como os pixels e inclusive colocar valores negativos. Além disso, existem palavras reservadas que facilitam no posicionamento do eixo x e y da imagem, tais como: right, left, center, top, bottom, start, end.
```













