# LAB-SFARI-DATASET-GENE

Análise de dados do dataset do [SFARI](https://gene.sfari.org/) para o LAB HCPA com a Professora Carmem.

## Instalação e importação de bibliotecas (as bibliotecas utilizadas)
* [pandas](https://pandas.pydata.org/)
* [opendatasets](https://pypi.org/project/opendatasets/)
     
## Acessando o arquivo CSV
* Vamos utilizar o comando od.download, colocando diretamente o link do arquivo que queremos. Se precisar inserir um username e uma key, é só inserir na caixa de texto que irá abrir.
* Com o Pandas, vamos ler o arquivo csv, utilizando o encoding LATIN1, devido aos nossos caractéres próprios.

## Recodificação dos dados
* Um dos grandes problemas dos arquivos DBF(caso use ele)/CSV é a codificação das variáveis. Simplesmente abrir o arquivo não traz informações claras, pois acabamos tendo que recorrer ao Dicionário de Dados daquele arquivo. Com o Python, conseguimos recodificar as colunas, escrevendo o dicionário de dados para cada uma. É um trabalho que leva algum tempo, porém, precisamos fazê-lo somente uma vez e depois já estará pronto.
* Avaliando o dicionário de dados, percebemos que muitas variáveis apresentam apenas o SIM e o NÃO. Para essas, faremos apenas um mini dicionário e aplicaremos a função REPLACE, que vai substituir os valores encontrados na tabela por aqueles vistos no dicionário.
* Utilizaremos uma coluna como exemplo, e depois aplicamos para as demais. Caso se queira alterar diversas colunas com a mesma informação, criaremos uma lista com as colunas que possuem codificação de SIM/NÃO, e aplicaremos uma das funções mais úteis do Python, o loop de repetição chamado de FOR.
Essa função nos permite aplicar diversas vezes a mesma operação, alterando apenas um parâmetro.
Deixei com # pois não utilizaremos nessa tabela, mas o código está aí se precisar.

     
## Renomeando as colunas

## Exportação para csv
* Caso queira exportar o novo DataFrame para csv, caso haja a necessidade de visualizar os dados em um programa. Esta operação demora um pouco.
     
## Aplicação de filtros
* Uma coisa que muitas vezes fazemos ao analisar um banco de dados, é um filtro.
* Declarar o filtro, e depois vamos aplicá-lo.
* E se quisermos fazer um DataFrame com mais de um parâmetro de filtro? Algumas maneiras de fazer:
* Fazer um filtro seguido do outro - desvantagem é que não podemos utilizar parâmetros dentro da mesma coluna, como por exemplo selecionar mais de uma coluna.
* Filtro composto: é o melhor jeito de fazer, podendo colocar filtros com E (&) / OU ( | )
* Filtro composto para a mesma coluna, criando uma lista: quando queremos fazer um filtro que é sempre na mesma coluna, mas temos vários itens. Aplica-se o filtro utilizando a função isin

## Criar os filtros

## Juntar os filtros

## Aplicar o filtro composto
* Filtro composto para a mesma coluna, criando uma lista: quando queremos fazer um filtro que é sempre na mesma coluna, mas temos vários itens. Aplica-se o filtro utilizando a função isin

## Criar a lista de cromossomos


## Definir o filtro


## Aplicar filtro


# Análises
  ## Contagem de valores

  ## Tabela dinâmica

#$ Visualização de dados
As principais bibliotecas utilizadas para visualização de dados atualmente são a Matplotlib e a Seaborn.

Matplotlib - é a biblioteca padrão do Python, que faz rodar quase todas as visualizações;
Seaborn - biblioteca que já faz algumas operações além de apenas plotar o gráfico, como adicionar rótulos nos eixos automaticamente, além de possuir muitos exemplos de gráficos muito bonitos.
Referências: https://python-graph-gallery.com/

Immportar bibliotecas.
