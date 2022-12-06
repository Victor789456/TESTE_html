-------------------------------------------------------------------------------------
DISCIPLINA: IEF829-INFORMÁTICA NO ENSINO DE FÍSICA | AULA 03 | DATA: 06/12/2022
-------------------------------------------------------------------------------------
EDIÇÃO DE TEXTO: HTML BÁSICO
-------------------------------------------------------------------------------------
MATERIAL COMPLEMENTAR DA AULA PRÁTICA
-------------------------------------------------------------------------------------
PROFESSOR: JOZIANO MIRANDA
-------------------------------------------------------------------------------------

Parte desse material foi organizado com base na fonte: 
https://www.tc.df.gov.br/ice4/vordf/outros/html-comandos.html

#### HTML (Hypertext Markup Language [Linguagem de Marcação Hipertexto]) ############

A HTML é baseada em marcações chamadas tags.

##### Estrutura básica de um documento HTML #########################################

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-sacale=1.0">
    <title>Título</title>    
</head>

<body>

</body>
</html>

##### tags de título ################################################################

<h1> Este é um título nível 1 </h1>
<h2> Este é um título nível 2 </h2>
<h3> Este é um título nível 3 </h3>
<h4> Este é um título nível 4 </h4>
<h5> Este é um título nível 5 </h5>
<h6> Este é um título nível 6 </h6>

##### tag parágrafo #################################################################

<p>
Este é o primeiro parágrafo do texto. Este é o primeiro parágrafo do texto.
Este é o primeiro parágrafo do texto. Este é o primeiro parágrafo do texto.
</p>

##### tags para alinhamento de texto ################################################

Alinhamento a esquerda (Padrão):
<p align="Left"> 
Insira aqui o texto
</p>

Alinhamento centralizado:
<p align="center"> 
Insira aqui o texto
</p>

Alinhamento a direita:
<p align="Right"> 
Insira aqui o texto
</p>

Alinhamento justificado:
<p align="Justify"> 
Insira aqui o texto
</p>

##### tag para colocar texto em negrito #############################################

<b> Insira aqui o texto </b> 

##### tag para colocar texto em itálico #############################################

<i> Insira aqui o texto </i>

##### tag para colocar texto sublinhado #############################################

<u> Insira aqui o texto </u>

##### tag para configurar a cor do texto [parte do texto] ###########################

<font color="cor"> Insira aqui o texto </font>

##### tag para especificar a cor do texto inteiro ###################################

Deve-se adicionar o atribulto na tag <body>
Exemplo: <body text="cor">

##### tag para configurar a cor de plano de fundo ###################################

Deve-se adicionar o atribulto na tag <body>
Exemplo: <body bgcolor="cor">

##### tag para adicionar quebra de linha ############################################

<br> Texto </br>

##### tag para criar um separador ou linha horizintal ###############################

<hr> 

##### tag para inserir links ########################################################

Método 1: <a href="https://ufam.edu.br/"> Visite o site da UFAM </a>
Método 2: <a href="https://ufam.edu.br/" target="_blank"> Visite o site da UFAM </a>

#### cor dos links ##################################################################

Azul é a cor padrão para links. Mas você pode alterar as cores dos seus links, 
inserindo estas tags dentro da tag <body>:

link="cor"
vlink="cor"

Vlink são os "links visitados". Os links mudam de cor quando foram visitados.
Se você não quiser que os links visitados mudem de cor, basta atribuir a mesma cor 
ao links e vlinks. 

##### tag para controlar o tamanho da fonte #########################################

<font size="tamanho"> Insira aqui o texto </font> 
OBS: O tamanho de fonte padrão na maioria dos navegadores é "3"

Método alternativo 1: mudar o tamanho de fonte ao somar ou subtrair números do 
tamanho padrão. Exemplo: <font size=+4> TEXTO </font> ou <font size=-2> TEXTO </font> 

método alternativo 2: usando as tags <small> TEXTO </small> ou <big> TEXTO </big>.

##### tag para listas ###############################################################

Uma lista desordenada tem marcadores e começa com a tag <ul> (abreviação de unordered list). 
A tag <li> (abreviação de List Item, ou item da lista) é usada antes de cada item da lista. 
A tag de fechamento </ul> encerra a lista.

Exemplo:

<ul>
<li> Item 1 da lista
<li> Item 2 da lista
<li> Item 3 da lista
</ul> 

O tipo de marcador pode ser trocado por "circle" (círculo), "square" (quadrado) ou 
"disc" (disco), adicionando uma especificação dentro da tag <ul>

Exemplos:

<ul type="circle">
<li> Item 1 da lista
<li> Item 2 da lista
<li> Item 3 da lista
</ul>

<ul type="square">
<li> Item 1 da lista
<li> Item 2 da lista
<li> Item 3 da lista
</ul> 

<ul type="disc">
<li> Item 1 da lista
<li> Item 2 da lista
<li> Item 3 da lista
</ul> 

Uma lista ordenada é uma lista de itens em uma ordem lógica numérica. 
Use as tags <ol> (abreviação de ordered list) e </ol> para começar e 
terminar este tipo de lista. A tag <li> também é usada na frente de cada item.

Exemplo:

<ol>
<li> Item 1 da lista
<li> Item 2 da lista
<li> Item 3 da lista
</ol>

O tipo de organização pode ser alterado, adicionando uma designação de "tipo" 
dentro da tag <ol>.

<ol type="A"> ordena a lista com letras maiúsculas: (A, B, C...)

<ol type="a"> ordena a lista com letras minúsculas: (a, b, c...)

<ol type="I"> ordena a lista com números romanos: (I, II, III...)

<ol type="i"> ordena a lista com números romanos minúsculos: (i, ii, iii...)

##### tag para inserir imagem #######################################################

se a imagem estiver na pasta do documento HTML:
<img src="nomeDaImagem.formato" alt="descrição da imagem">

Se a imagem estiver em uma pasta separada do documento HTML:
<img src="nomeDaPasta/nomeDaImagem.formato" alt="descrição da imagem">

Se a imagem for de um site da internet:
<img src="endereçoWebDaImagem" alt="descrição da imagem">

Se deseja-se controlar a largura e a altura da imagem:
<img src="nomeDaImagem.formato" alt="descrição da imagem" width=300 height=200>

onde: width = largura e height = altura

Para alinhar a imagem (esquerda [padrão], direita e centro), basta
usar a tag imagem dentro da tag de paragrafo com o respectivo alinhamento, 
por exemplo:

<p align="center">
<img src="imagens/img.jpeg" alt="descrição da imagem">
</p>

##### tag para inserir link na imagem ################################################

<a href="site" target="_blank">
<img src="nomeDaImagem.formato" alt="descrição da imagem">
</a>
