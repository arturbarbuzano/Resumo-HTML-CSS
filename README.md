# GuiaRapido-HTML-CSS

Este documento apresenta um resumo simples e direto dos principais conceitos de HTML e CSS.

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










