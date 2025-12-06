# GuiaRapido-HTML-CSS

Este documento apresenta um resumo simples e direto dos principais conceitos de HTML e CSS.

## HTML

```sh
<!DOCTYPE html> ---> Use versão HTML5
<html> </html> ---> Arquivo HTML
<head> </head> ---> Cabeça do Arquivo
<body> </body> ---> Corpo do Arquivo
<title> </title> ---> Título do Documento
<meta charset="UTF-8"> ---> Evita erros de Acentuação
<meta name="viewport" content="width=device-width, initial-scale=1.0"> ---> Responsividade
<link href="caminho" rel="stylesheet"> ---> Linkar com Arquivo CSS
<style> </style> ---> Estilização CSS

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

<h1> </h1> ---> Cabeçalho Um
<p> </p> ---> Parágrafo
<br> ---> Pula Linha
<hr> ---> Cria linha Divisão
<strong> </strong> ---> Negrito Semântico
<small> </small> ---> Pequeno
<i> </i> ---> Itálico

<a href="URL">Nome</a> --> Link
<img src="caminho" alt="descrição (acessibilidade" width="largura" height="altura"> ---> Imagem
<video src="caminho" width="largura" controls(adiciona controles:play, pause, volume)></video>
<audio src"caminho" controls(adiciona controles:play, pause, volume)></audio>
<iframe src="URL" width="largura"> </iframe> ---> Página dentro de outra Página

<ol> ---> Lista Ordenada
  <li> </li> --> Item da Lista
  <li> </li> --> Item da Lista
</ol> ---> Lista Ordenada
<ul> ---> Lista Não Ordenada
  <li> </li> --> Item da Lista
  <li> </li> --> Item da Lista
</ul> ---> Lista Não Ordenada

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









