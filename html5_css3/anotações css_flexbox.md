# CSS Flexbox
criacao de paginas com layout e distribuicao de espaçcos que se adaptam a diversos layouts

Flex container é o item principal que pode ser subdividido em Flex Itens

Display flex
é uma tag que cria um container e torna tudo abaixo dele como filhos diretos dessa tag

Flex direction
estabelece eixos do container

LINHA
row - escrita da esquerda para a direita - 1 2 3 4
row-reverse - escrita no sentido oposto, da direita p esquerda - 4 3 2 1

COLUNA
column: ordenacao de cima para baixo
column-reverse: ordenaçao de baixo para cima

Flex wrap
define ou nao a quebra de linha do nosso container porque por padrao eles nao quebram linha e começa a vazar do container qdo excede

wrap - quebra a linha para baixo, sempre seguindo a sequencia logica da escrita, de cima para baixo
wrap-reverse: quebra a linha para cima, subindo o texto de baixo para cima

Flex flow
é um atalho para flex direction e flex wrap porem o seu uso nao é muito comum

Justify content
vai se encarregar do alinhamento e distribuicao de espacamento entre os itens do container
caso o item ja ocupa 100% do container nao faz sentido usar
flex-start
flex-end
center
space-between
space-around

Align Items
trata o alinhamento dos itens de acordo com o eixo dos containers
center
stretch
flex-start
flex-end
baseline

Align Content
trata o alinhamento dos itens de acordo com o eixo vertical dos containers
center
stretch
flex-start
flex-end
space-between
space-around

Propriedades relacionadas ao flex items

flex grow
define a proporcao de crescimento dos itens, respeitando o tamanho do conteudo interno  
OBS: nao funciona com justify content aplicado ao container

flex basis
define o tamanho minimo do item antes da distrbuicao do espaco
auto
px ou % =  valor exato
0 (zero) = definicao ligada com flexgrow    

Flex Shrink
define a reducao ou compressao do tamanho de um item

Flex
é um atalho para as propriedades grow, shrink e basis nessa ordem

Order
define a ordenação dos itens

align self
define o alinhamento individual de cada item, podendo definir o padrao de cada um individual. o container nao pode ter o align item definido.
auto
flex-start
flex-end
center
strecth
baseline