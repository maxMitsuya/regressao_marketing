# Desafio: Construindo um Modelo de Regressão para Marketing

Este projeto foi desenvolvido como parte de um desafio do curso DNC, para construir um modelo de regressão aplicado a dados de marketing. O objetivo é prever o retorno de vendas com base nos investimentos em plataformas de publicidade online, como YouTube, Facebook e Newspaper. O código foi criado e executado no **Google Colab**, utilizando bibliotecas populares de Python para análise de dados e machine learning.

## Contexto

Uma empresa investe mensalmente em plataformas de publicidade online (YouTube, Facebook e Newspaper) para prospectar leads (pessoas interessadas em seus produtos). Para acompanhar o desempenho desses investimentos, a empresa registra os gastos com publicidade e os retornos de vendas gerados. O objetivo deste projeto é:

1. **Entender a relação** entre os investimentos em diferentes plataformas e as vendas geradas.
2. **Identificar os fatores** que mais impactam na geração de vendas.
3. **Criar um modelo de predição** para estimar o retorno de vendas com base nos investimentos.

## Sobre os Dados

O dataset utilizado contém as seguintes colunas:

- **youtube**: Investimento em publicidade no YouTube.
- **facebook**: Investimento em publicidade no Facebook.
- **newspaper**: Investimento em publicidade em jornais.
- **sales**: Vendas geradas (variável alvo).

O dataset possui **171 registros**, sem valores nulos, e os tipos de dados estão corretos para cada coluna.

## Ferramentas e Tecnologias Utilizadas

- **Google Colab**: Ambiente de execução do código.
- **Python**: Linguagem de programação principal.
- **Bibliotecas**:
  - `pandas`: Para manipulação de dados.
  - `matplotlib` e `seaborn`: Para visualização de dados.
  - `plotly`: Para gráficos interativos.
  - `scikit-learn`: Para modelagem de machine learning (regressão linear, validação, métricas).

## Estrutura do Projeto

1. **Importação dos Dados**:
   - Carregamento do dataset `MKT.csv`.
   - Visualização das primeiras linhas do dataset.

2. **Análise Descritiva**:
   - Verificação de informações básicas do dataset (`info` e `describe`).
   - Identificação de outliers usando gráficos boxplot.

3. **Análise Exploratória de Dados (EDA)**:
   - Visualização da relação entre as variáveis usando pairplot.
   - Análise de correlação entre as variáveis usando heatmap.

4. **Modelagem dos Dados**:
   - Divisão dos dados em conjuntos de treino (70%) e teste (30%).
   - Treinamento de um modelo de regressão linear.
   - Predição dos valores de vendas no conjunto de teste.
   - Avaliação do modelo usando o coeficiente de determinação \( R^2 \).

5. **Visualização dos Resultados**:
   - Gráfico comparando os valores reais e previstos de vendas.

## Resultados

O modelo de regressão linear alcançou um coeficiente de determinação \( R^2 \) de **0.88**, indicando que 88% da variabilidade das vendas pode ser explicada pelos investimentos em YouTube, Facebook e Newspaper. Isso significa que, caso haja alterações positivas ou negativas nos investimentos, há 88% de chances de impactar as vendas de forma correspondente.

## Como Executar o Projeto

### No Google Colab

1. Clique no botão abaixo para abrir o notebook no Google Colab:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1BtOX0br3STae3qPS3hWBNyBeXC7kIj2P?usp=sharing)

2. Faça uma cópia do notebook na sua conta do Google Drive.
3. Execute as células na ordem para reproduzir os resultados.
