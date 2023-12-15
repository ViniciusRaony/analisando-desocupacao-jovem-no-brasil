# Análise exploratória de dados - Analisando a Desocupação da População Jovem no Brasil

A população jovem no Brasil, definida pela Lei nº 12.852 de 2013 - Estatuto da Juventude, como pessoas com idade entre 15 (quinze) e 29 (vinte e nove) anos de idade, enfrenta uma série de desafios significativos. Entre esses desafios, a desocupação se destaca como um problema persistente que afeta as perspectivas de futuro desses jovens.

Nesta análise, irei explorar um conjunto de dados que contém informações sobre população por idade e a taxa de desocupação dessa faixa etária no Brasil. A taxa de desocupação é a porcentagem de pessoas na força de trabalho que estão sem emprego. 

Ao analisar esses dados, podemos obter insights valiosos sobre as condições de vida e as perspectivas de futuro desses jovens. Isso pode nos ajudar a entender melhor o cenário atual da juventude no Brasil e identificar áreas onde podem ser necessárias intervenções ou políticas públicas adicionais.


<center><img alt="Colaboratory logo" width="35%" src="https://raw.githubusercontent.com/ViniciusRaony/analisando-desocupacao-jovem-no-brasil/main/images/img_desocupacao.jpg"></center>

Através desta análise, espero contribuir para uma melhor compreensão da desocupação da população jovem no Brasil, uma área que vem enfrentando desafios significativos nos últimos anos.


## Obtenção dos Dados
Os dados utilizados nesta análise foram obtidos a partir do site do IBGE. Os dados sobre a desocupação foram retirados da [Pesquisa Nacional por Amostra de Domicílios Contínua](https://sidra.ibge.gov.br/pesquisa/pnadct/tabelas) (PNAD Contínua), que fornece informações detalhadas sobre a desocupação no Brasil.

Além disso, os dados demográficos foram obtidos a partir do [Censo Demográfico de 2022](https://sidra.ibge.gov.br/pesquisa/censo-demografico/demografico-2022/universo-populacao-por-idade-e-sexo), que fornece informações sobre a população brasileira, incluindo idade e gênero.

No geral, os dados do IBGE já possuem um ótimo tratamento dos dados.

**Para facilitar o acesso, os dados brutos estão na pasta raw desse repostório.**

## Análise Exploratória dos Dados

Esta etapa tem por objetivo criar uma consciência situacional inicial e permitir um entendimento de como os dados estão estruturados.

Vamos importar os pacotes necessários e iniciar nossa Análise Exploratória.

**Dicionário das variáveis**

dataset IBGE - Censo 2022

* `Unidade da Federação` - Estado da Federação brasileira
* `0 a 4 anos` - população na faixa etária de 0 a 4 anos
* `...` - população nas faixas etárias subsequentes
* `100 anos ou mais` - população na faixa etária de 100 anos ou mais


dataset PNAD
* `Grupo de Idade` - Estado da Federação brasileira
* `Brasil e Unidade da Federação` - Estado da Federação brasileira + Brasil (total)
* `1º trimestre 2012` - taxa de desocupação do 1º trimestre de 2012
* `...` - taxas de desocupação dos trimestres subsequentes
* `3º trimestre 2023` - taxa de desocupação do 3º trimestre de 2023