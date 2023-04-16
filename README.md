# Aluguel de imóveis - Canadá

Porjeto aplica tecnicas de analise de dados a fim de entender e relacionar o mercado para que investidores e proprietários tenham maior visão estrategica akudando assim em suas tomadas de decisões.

Todos os dados foram retirados do portal da [Inside Airbnb](http://insideairbnb.com/get-the-data.html). Para esta análise utilizei o arquivo: `canada.csv`, onde no mesmo portal é encontrado uma base de dados bem maior e mais completa.

### Como foi feita a analise?
Primeiramente inportamos os pacotes e bibliotecas necessarias para analise.

[Pandas](https://pandas.pydata.org/) é uma biblioteca de software criada para a linguagem Python para manipulação e análise de dados. 
 
[Numpy](https://numpy.org/) é uma biblioteca para a linguagem de programação Python, que suporta o processamento de grandes, multi-dimensionais arranjos e matrizes, juntamente com uma grande coleção de funções matemáticas de alto nível para operar sobre estas matrizes.

[Matplotlib](https://matplotlib.org/)é uma biblioteca de software para criação de gráficos e visualizações de dados em geral, feita para e da linguagem de programação Python e sua extensão de matemática NumPy.

[Seaborn](https://seaborn.pydata.org/) é uma das mais poderosas ferramentas para plotagem dos mais variados tipos de gráficos em Python.

Depois de importar todos os pacotes necessarios, importei a base de dados usando [pandas](https://pandas.pydata.org/).

Coloquei um dicionario de variaveis com intuito de permitir um entendimento de como os dados estão estruturados.

![Screenshot_1](https://user-images.githubusercontent.com/33229102/232338434-877404dd-34c1-46ac-bcba-bbf29efd9c7c.png)

Apresentei um codigo para identificar o volume de dados. Entrada e tipos de variaveis que são basicamnete os valores das minhas linhas e colunas.

Ordenei em ordem decrescente as variáveis por seus valores ausentes.

Para identificar a distribuição das variáveis, plotei um histograma.

* `O histograma, também conhecido como distribuição de frequências, é a representação gráfica em colunas ou em barras de um conjunto de dados previamente tabulado e dividido em classes uniformes ou não uniformes.`

![Screenshot_4](https://user-images.githubusercontent.com/33229102/232339596-9738b0bf-f202-44c8-a6b6-5976b69c4cf6.png)

Pela distribuição do histograma, é possível verificar indícios da presença de outliers.

* `Os outliers são dados que se diferenciam drasticamente de todos os outros. Em outras palavras, um outlier é um valor que foge da normalidade e que pode (e provavelmente irá) causar anomalias nos resultados obtidos por meio de algoritmos e sistemas de análise.`

Para detectar os outliers usei um resumo estatístico por meio do método describe(), logo após plotei boxplots para a variável.

* `metodo describe: Esta função mostra estatísticas descritivas, como média, desvio padrão, máximo, mínimo e outras tendências centrais, além da forma da distribuição. Isso é útil para se ter uma ideia sobre a distribuição dos campos de dados e outliers, se houver.`

Logo após identificar os outliers limpo a dataframe delas e plotar novamente o histograma.

Crio uma matriz de correlação e gero um heatmap a partir dessa matriz, usando a biblioteca [seaborn](https://seaborn.pydata.org/).

* `Correlação significa que existe uma relação entre duas coisas. No nosso contexto, estamos buscando relação ou semelhança entre duas variáveis.`

![Screenshot_5](https://user-images.githubusercontent.com/33229102/232340385-9f5e7d71-fa39-4870-8f85-f43e2f436010.png)

Crio um codigo que mostrar a quantidade de cada tipo de imóvel disponível e comparo cos bairros mais caros.

Por ultimo ploto os imóveis pela latitude-longitude. 

![Screenshot_6](https://user-images.githubusercontent.com/33229102/232340560-99afa6af-c8e5-432e-9334-e4e25702ba0f.png)

### Conclusão

A análise exploratória dos dados revelou que o preço do aluguel de casas no Canadá está fortemente relacionado com a localização, tamanho da propriedade e número de quartos. A partir desses resultados, é possível usar técnicas de análise de dados e machine learning para facilitar a busca por imóveis para aluguel no país. Além disso, a análise também pode ajudar investidores e proprietários a tomar decisões estratégicas no mercado imobiliário.

# Autor:

<div>
<a href="https://www.linkedin.com/in/marcelo-maia-dev" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>     
<a href = "mailto:marcelo.maia962@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
</div>


