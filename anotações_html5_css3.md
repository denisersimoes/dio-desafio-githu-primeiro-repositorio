# Anotações de Aula 

# HTML 5

### Historia e estrutura basica

**HTML5**

Definição e estrutura básica

Em 1991 Tim Berners-Lee criou essa linguagem de marcação para melhorar a comunicação entre ele e seus colegas de trabalho no CERN, desde então já surgiram 5 versões e o HTML se tornou a base da web.

Com o HTML definimos o significado e a estrutura do conteúdo da web e, além de texto, nossas páginas precisam de imagens, vídeos e vários outros formatos e para isso temos os elementos HTML.

Um elemento HTML é formado pela tag de abertura e seus atributos, o conteúdo e uma tag de fechamento. E mais a frente veremos que existem elementos que não tem tag de fechamento.

 ![elemento HTML](/images/elemento_html.jpg)

Com esses elementos podemos agrupar tipos de conteúdo, alterar tamanho e forma de fontes e adicionar diferentes mídias ao nossa página na web.

E agora podemos ver como é a estrutura básica de um arquivo HTML.

 ![estrutura HTML](/images/estrutura_basica_html.jpg)

## Exercicio Pratico
Criada uma pagina chamada index.html para verificar os conceitos aplicados

- TAG DOCTYPE

 A primeira linha do documento deve ser o !DOCTYPE html, apesar de parecer um elemento HTML ela apenas diz ao navegador que ele está lidando com um arquivo do tipo HTML5. Os elementos HTML vem logo abaixo.

- TAG HTML

A tag html é a raiz do seu documento, todos os elementos HTML devem estar dentro dela. E nela nós informamos ao navegador qual é o idioma desse nosso documento, através do atributo lang, para o português brasileiro usamos pt-BR.

- TAG HEAD

A tag head contém elementos que serão lidos pelo navegador, como os metadados - um exemplo é o charset, que é a codificação de caracteres e a mais comum é a UTF-8, o JavaScript com a tag script, o CSS através das tags style e link - veremos a diferença quando falarmos sobre CSS - e o título da página com a tag title.

- TAG BODY

E dentro da tag body colocamos todo o conteúdo visível ao usuário: textos, imagens, vídeos.

# Semântica
Durante muitos anos o elemento padrão no HTML era a div, construíamos nosso conteúdo todo baseado nela, e assim nascia a sopa de divs.

Mas em 2014 saiu a quinta versão do HTML, e com ela vieram vários mudanças importantes, como performance e acessibilidade, mas nesse curso introdutório vamos focar na semântica.

A semântica nos permite descrever mais precisamente o nosso conteúdo, agora um bloco de texto não é apenas uma div, agora é um article e tem mais significado assim. E temos vários elementos para ressignificar as divs:

- Elemento section

Representa uma seção genérica de conteúdo quando não houver um elemento mais específico para isso.

- Elemento header

É o cabeçalho da página ou de uma seção da página e normalmente contém logotipos, menus, campos de busca.

- Elemento article

Representa um conteúdo independente e de maior relevância dentro de uma página, como um post de blog, uma notícia em uma barra lateral ou um bloco de comentários. Um article pode conter outros elementos, como header, cabeçalhos, parágrafos e imagens.

- Elemento aside

É uma seção que engloba conteúdos relacionados ao conteúdo principal, como artigos relacionados, biografia do autor e publicidade. Normalmente são representadas como barras laterais.

- Elemento footer

Esse elemento representa o rodapé do conteúdo ou de parte dele, pois ele é aceito dentro de vários elementos, como article e section e até do body. Exemplos de conteúdo de um footer são informações de autor e links relacionados.

- Elementos h1 até h6

Eles não foram criados na versão 5 do HTML e nem são específicos para semântica, mas servem para esse propósito. São utilizados para marcar a importância dos títulos, sendo h1 o mais importante e h6 o menos. Uma dica: use apenas um h1 por página, pois ele representa o objetivo da sua página.

## Exercicio Pratico
Adicionar essa nova estrutura na pagina index.html ja criada

## Textos e links
- Elemento p

O p representa um parágrafo, mas ele não suporta apenas texto, podemos adicionar imagens, código, vídeos e vários outros tipos de conteúdo dentro dele.

- Elemento a

Um outro elemento interessante e extremamente necessário na web é o a que significa anchor/âncora, ele representa um hyperlink, é ele que interliga vários conteúdos e páginas na web.

O elemento a tem vários atributos, mas vamos focar em dois, o href e o target.

O href representa o hyperlink para onde sua âncora aponta, pode ser uma página do seu ou de outro site, um e-mail e até mesmo um telefone, os dois últimos precisam dos prefixos mailto: e tel:, respectivamente.

O target neste momento vai servir para nos ajudar a abrir nossos links em outra aba do navegador usando o valor _blank.

## Exercicio Prático
Adicionar um texto fictício na pagina index.html, inserir o elemento p com um texto qualquer e inserir dois elementos a colocando um link para outra página e um para nosso e-mail.

## Imagens
A web também é feita de imagens e para representá-las temos o elemento img, ele é um daqueles elementos sem tag de fechamento.

O elemento img é bem simples, contendo apenas 2 atributos próprios, o src e o alt.

O src é obrigatório e guarda o caminho para a imagem que você quer mostrar na página.

O alt não é obrigatório mas é altamente recomendado por melhorar a acessibilidade, ele mostra a descrição da imagem caso ela não carregue e leitores de tela usam esse atributo para descrever a imagem para o usuário saber o que ela significa.

## Exercicio Pratico
Vamos adicionar na nossa pagina index.html uma imagem ao cabeçalho e uma imagem a postagem.

## Listas
Os últimos elementos que veremos neste módulo são os relacionados a listas: ul, ol e li.

Listas servem para agrupar uma coleção de itens, como uma lista de ingredientes ou, como será no nosso caso, uma lista com contatos.

O elemento ul cria uma lista não ordenada, onde a ordem dos elementos não é importante, e é representada com pontos, círculos ou quadrados.

O elemento ol serve para criar lista ordenadas, nessas a ordem importa, portanto elas são representadas com números, algarismos romanos ou letras.

E o elemento li é um item dentro de uma dessas listas. Um li pode conter vários tipos de conteúdos, como parágrafos, imagens e até outras listas.

## Exercicio Pratico
Vamos adicionar na nossa pagina index.html, no nosso rodapé, uma lista de contatos nao ordenado e uma lista de contatos ordenado.

# CSS3
1996 foi criada essa sintaxe para formatação do HTML

## Seletores
sao os parametros ja utilizados no HTML
exemplo elementos P, a, h1, h3
apos a indicacao do elemento, é inserido um par de chaves {} para inserir as declarações que sao a formatacao desejada.
podemos definir a cor, atraves da declaracao COLOR
podemos definir o tamanho da letra atraves da declacarao FONT-SIZE

para definir formatacoes diferentes para o mesmo elemento html (seletor) usamos ID e CLASSES diferentes

no HTML a gente define o ID usando a palavra ID apos o seletor desejado
e define a CLASSE usando a palavra CLASS apos o seletor desejado

no CSS uma CLASSE é precedida por um .(ponto) e um ID é precedido por #(jogo da velha ou hash)
ID só pode ser usado 1 vez na pagina

## Exercicio Pratico
