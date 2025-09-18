### 📝 Resumo do Projeto: Análise Preditiva de Doenças Cardíacas

Este projeto realiza uma análise completa do dataset "Heart Disease" com o objetivo de construir um modelo de classificação capaz de prever a presença de doenças cardíacas em pacientes com base em um conjunto de atributos clínicos.

O fluxo de trabalho seguiu as seguintes etapas:

1.  **Limpeza e Pré-processamento de Dados:**
    * Identificação e remoção de **723 registros duplicados**, resultando em um dataset final com 302 entradas únicas.
    * Tratamento de *outliers* em colunas numéricas (`trestbps`, `chol`, `thalach`) utilizando a técnica de quantil para garantir a robustez dos dados.

2.  **Análise Exploratória de Dados (EDA):**
    * Visualização da distribuição de cada variável para compreender suas características.
    * Análise de correlação entre os atributos para identificar relações lineares.
    * Geração de gráficos para comparar a distribuição das variáveis categóricas em relação à variável alvo (`target`).

3.  **Engenharia de Features e Modelagem:**
    * Conversão de variáveis categóricas em formato numérico através de *One-Hot Encoding* (`pd.get_dummies`) para preparar os dados para os algoritmos.
    * Divisão do dataset em conjuntos de **treino e teste** (proporção 80/20).
    * Treinamento e avaliação de múltiplos modelos de Machine Learning, incluindo:
        * Regressão Logística
        * Árvore de Decisão
        * AdaBoost
        * Random Forest
        * K-Nearest Neighbors (KNN)

4.  **Avaliação dos Modelos:**
    * A performance de cada classificador foi metrificada utilizando **Acurácia**, **Classification Report** (precisão, recall, F1-score) e **Matriz de Confusão** para avaliar a capacidade de predição em dados não vistos.
