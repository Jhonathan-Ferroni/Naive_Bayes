# Classificação com Naive Bayes - Análise de Dados com `insurance.csv`

Este projeto implementa um modelo de classificação utilizando o algoritmo **Naive Bayes Gaussiano** para prever categorias com base em um conjunto de dados do setor de seguros. O código faz o pré-processamento dos dados, aplica transformações para lidar com variáveis categóricas, divide os dados em treino e teste, e avalia a performance do modelo com diversas métricas.

## Objetivo
O objetivo deste projeto é criar um modelo de classificação que consiga prever corretamente a categoria de um evento com base em variáveis independentes do dataset `insurance.csv`.

## Estrutura do Projeto
O script Python está organizado nas seguintes etapas:

### 1. Importação de Bibliotecas
- `pandas` para manipulação de dados.
- `sklearn.model_selection` para dividir os dados entre treino e teste.
- `sklearn.naive_bayes` para aplicar o modelo Naive Bayes Gaussiano.
- `sklearn.preprocessing` para codificação de variáveis categóricas.
- `sklearn.metrics` para avaliação do desempenho do modelo.
- `yellowbrick.classifier` para visualização da matriz de confusão.

### 2. Carregamento e Preparação dos Dados
- Leitura do arquivo `insurance.csv`.
- Remoção de colunas desnecessárias.
- Tratamento de valores ausentes, substituindo `NaN` por `None`.
- Separar as variáveis independentes (`X`) e a variável dependente (`y`).
- Aplicar `LabelEncoder` para transformar variáveis categóricas em valores numéricos.

### 3. Divisão dos Dados
- Divisão dos dados em **70% para treino** e **30% para teste** utilizando `train_test_split()`.

### 4. Treinamento do Modelo
- Criar e treinar um modelo de **Naive Bayes Gaussiano** (`GaussianNB`).
- Fazer previsões com os dados de teste.

### 5. Avaliação do Modelo
- Calcular **acurácia, precisão, recall e F1-score**.
- Exibir um **relatório de classificação** (`classification_report`).
- Gerar graficamente a **matriz de confusão** com `yellowbrick`.

## Requisitos
Certifique-se de ter as bibliotecas necessárias instaladas:

```bash
pip install pandas scikit-learn yellowbrick
```

## Como Executar
1. Clone este repositório:

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. Certifique-se de que o arquivo `insurance.csv` esteja no mesmo diretório do script.

3. Execute o script Python:

   ```bash
   python naivebayes.py
   ```

## Dataset
O dataset `insurance.csv` contém informações sobre registros de seguros e seus atributos. Algumas das colunas presentes incluem:

- `age`: Idade do cliente.
- `sex`: Sexo do cliente.
- `bmi`: Índice de massa corporal.
- `children`: Número de filhos.
- `smoker`: Indica se o cliente é fumante.
- `region`: Região onde o cliente reside.
- `charges`: Custos do seguro.

## Resultados Esperados
Ao final da execução do script, espera-se obter:

- Um modelo de classificação treinado.
- Métricas de desempenho do modelo (acurácia, precisão, recall, F1-score).
- Matriz de confusão para avaliação visual.


---

Contribuições e sugestões são bem-vindas! 😊

