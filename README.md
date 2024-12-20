# Lab House Pricing Machine Leaning(Regression)
In this assignment, you are a Data Analyst working at a Real Estate Investment Trust. The Trust would like to start investing in Residential real estate. You are tasked with determining the market price of a house given a set of features. You will analyze and predict housing prices using attributes or features such as square footage, number of bedrooms, number of floors, and so on.

# House Sales in King County, USA
This notebook analyzes house sale prices in King County, USA, including Seattle. It uses a dataset of homes sold between May 2014 and May 2015 to explore data, develop models for price prediction, and evaluate their performance.

## Workflow and Steps
## **1- Data Collection and Understanding:**
  - The dataset is imported from a ´CSV file´.
  - Initial data exploration is performed to understand the features, data types, and basic statistics.

## **2- Data Wrangling:**
 - Unnecessary columns ('id', 'Unnamed: 0') are removed.
 - Missing values in 'bedrooms' and 'bathrooms' are imputed using the mean of their respective columns.

## **3- Exploratory Data Analysis (EDA):**

- The distribution of unique floor values is analyzed.
  - Box plots are used to visualize price outliers based on waterfront view presence.
  - Regression plots examine the correlation between 'sqft_above' and price.
  - Correlation analysis identifies the features most correlated with price.

## **4- Model Development:**

- Linear regression models are built and evaluated using different feature sets:
  - 'long' feature only
  - 'sqft_living' feature only
  - A set of selected features (floors, waterfront, lat, bedrooms, sqft_living, view, bathrooms, sqft_living15, sqft_above, grade)
  - A pipeline is created with StandardScaler, PolynomialFeatures, and LinearRegression to potentially improve model performance.

## **5- Model Evaluation and Refinement:**

- Data is split into training and testing sets.
  - Ridge regression is applied with regularization to potentially improve model generalization.
  - Polynomial transformation is considered to capture non-linear relationships in the data.
  - R^2 scores are used to evaluate model performance on the test set.
- Usage
  - Make sure you have the necessary libraries installed (pandas, matplotlib, seaborn, scikit-learn).
  - Run the notebook cells sequentially to follow the workflow.
  - Experiment with different features, models, and hyperparameters to explore potential improvements.


## ***Português-BR***
# **Vendas de Casas em King County, EUA** 
Este notebook analisa os preços de venda de casas em King County, EUA, incluindo Seattle. Ele utiliza um conjunto de dados de casas vendidas entre maio de 2014 e maio de 2015 para explorar os dados, desenvolver modelos para previsão de preços e avaliar seu desempenho.

# **Fluxo de Trabalho e Etapas**

## **1- Coleta e Compreensão de Dados:**
  - O conjunto de dados é importado de um arquivo CSV.
  - Uma exploração inicial dos dados é realizada para entender as características, tipos de dados e estatísticas básicas.

## **2- Tratamento de Dados:**
  - Colunas desnecessárias ('id', 'Unnamed: 0') são removidas.
  - Valores ausentes em 'bedrooms' e 'bathrooms' são imputados usando a média de suas respectivas colunas.
  - Análise Exploratória de Dados (EDA):

## **3- A distribuição de valores únicos de andares é analisada.**
 - Box plots são usados para visualizar outliers de preços com base na presença de vista para a orla.
 - Gráficos de regressão examinam a correlação entre 'sqft_above' e preço.
 - A análise de correlação identifica as características mais correlacionadas com o preço.

## **4- Desenvolvimento de Modelo:**
- Modelos de regressão linear são construídos e avaliados usando diferentes conjuntos de características:
  - Apenas a característica 'long'
  - Apenas a característica 'sqft_living'
  - Um conjunto de características selecionadas (floors, waterfront, lat, bedrooms, sqft_living, view, bathrooms, sqft_living15, sqft_above, grade)
  - Um pipeline é criado com StandardScaler, PolynomialFeatures e LinearRegression para potencialmente melhorar o desempenho do modelo.

## **5- Avaliação e Refinamento do Modelo:**
- Os dados são divididos em conjuntos de treinamento e teste.
  - A regressão Ridge é aplicada com regularização para potencialmente melhorar a generalização do modelo.
  - A transformação polinomial é considerada para capturar relações não lineares nos dados.
  - As pontuações R^2 são usadas para avaliar o desempenho do modelo no conjunto de teste.
