# 📊 Predição de Evasão de Clientes (Churn) - Projeto de Data Science

## 📌 Descrição do Projeto

Este projeto tem como objetivo analisar e prever a evasão de clientes
(*Churn*) em uma empresa de telecomunicações.\
A partir de um conjunto de dados de clientes, foram realizadas etapas de
**pré-processamento, exploração, modelagem e avaliação** de modelos de
Machine Learning para identificar os fatores que mais influenciam a
saída de clientes e propor estratégias de retenção.

------------------------------------------------------------------------

## 🚀 Etapas do Projeto

### 1. Importação e Preparação dos Dados

-   Fonte: Dataset disponível no GitHub.\
-   Seleção das colunas mais relevantes para a análise.\
-   Conversão da variável alvo `Churn` para formato binário (0 = ativo,
    1 = evadido).\
-   Tratamento de valores ausentes com **SimpleImputer**.\
-   Codificação de variáveis categóricas via **One-Hot Encoding**.\
-   Padronização de variáveis numéricas com **StandardScaler**.

### 2. Análise Exploratória

-   Cálculo da **proporção de clientes evadidos vs ativos**
    (identificação de desequilíbrio de classes).\
-   Análise de **correlação entre variáveis numéricas e churn**.\
-   Visualizações:
    -   Boxplots: `tenure`, `MonthlyCharges`, `TotalCharges` vs Churn.\
    -   Scatter plots para explorar tendências.

### 3. Modelagem Preditiva

Foram aplicados dois algoritmos:\
- **Regressão Logística**\
- **K-Nearest Neighbors (KNN)**

Os dados foram divididos em **treino (70%)** e **teste (30%)**,
utilizando **stratify** para balanceamento da variável alvo.

### 4. Avaliação dos Modelos

As métricas utilizadas foram:\
- **Acurácia**\
- **Precisão**\
- **Recall (Sensibilidade)**\
- **F1-Score**\
- **Matriz de Confusão**

### 5. Resultados Obtidos

-   **Regressão Logística**: melhor desempenho com acurácia de \~79% e
    recall de 55%.\
-   **KNN**: desempenho inferior, com acurácia de \~75% e recall de
    48%.\
-   A Regressão Logística se mostrou mais eficiente para prever clientes
    em risco de evasão.

### 6. Principais Fatores Identificados

-   **Tipo de contrato** (contratos mensais têm maior churn).\
-   **Método de pagamento** (boleto associado a maior evasão).\
-   **Serviços adicionais de internet** (ausência aumenta o churn).\
-   **Tempo de permanência (tenure)** (clientes novos são mais propensos
    a sair).\
-   **Perfil de gastos** (clientes com mensalidades altas no início
    tendem a cancelar).

### 7. Estratégias de Retenção Propostas

-   Incentivar contratos de longo prazo.\
-   Oferecer pacotes de serviços adicionais.\
-   Personalizar preços e benefícios para novos clientes.\
-   Incentivar uso de pagamentos automáticos.\
-   Criar programas de fidelidade e engajamento.

------------------------------------------------------------------------

## 🛠️ Tecnologias Utilizadas

-   **Python 3**\
-   **Pandas, NumPy** (manipulação de dados)\
-   **Matplotlib, Seaborn** (visualização de dados)\
-   **Scikit-Learn** (pré-processamento, modelagem e métricas)

------------------------------------------------------------------------

## 📈 Conclusão

O projeto mostrou que é possível identificar padrões de evasão e
antecipar o comportamento dos clientes com boa precisão utilizando
**Regressão Logística**.\
As análises forneceram insights valiosos para o negócio, permitindo
definir estratégias de retenção personalizadas.

------------------------------------------------------------------------

## 📂 Estrutura do Projeto

    ├── dados_tratados.csv     # Dataset utilizado
    ├── notebooks/             # Notebooks do Google Colab
    ├── README.md              # Documentação do projeto

------------------------------------------------------------------------

📌 **Autor:** *\[Seu Nome\]*\
📌 \*\*Projeto acadêmico/desafio inspirado em estudos de Data Science e
Machine Learning.\*
