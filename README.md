# Modelo de Predição de Churn para Academias

[![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🎯 Objetivo do Projeto

Este projeto foca na aplicação de técnicas de **Ciência de Dados** e **Machine Learning** para prever a probabilidade de *churn* (cancelamento de matrícula) em clientes de academias e centros de fitness. O objetivo principal é identificar membros com alto risco de evasão, permitindo a implementação de estratégias de retenção personalizadas e eficazes para melhorar a sustentabilidade do negócio.

Este repositório demonstra habilidades em:

*   Análise Exploratória de Dados (EDA) específica para o setor fitness.
*   Pré-processamento de dados (limpeza, tratamento de dados faltantes, feature scaling).
*   Engenharia de Features (criação de variáveis relevantes como frequência de uso, tipo de plano, tempo de contrato, etc.).
*   Treinamento e avaliação de modelos de classificação (Regressão Logística, SVM, Random Forest, Gradient Boosting).
*   Interpretação de modelos para entender os fatores que mais influenciam o churn.
*   Visualização de dados para comunicação de insights.

## Features Principais

*   **Análise de Dados Específica:** Investigação de padrões de frequência, uso de instalações, tipos de planos e dados demográficos.
*   **Modelagem Preditiva:** Construção de modelos para classificar clientes como 'Churn' ou 'Não Churn'.
*   **Avaliação Robusta:** Uso de métricas apropriadas (Recall, Precision, F1-Score, AUC) para lidar com possíveis desbalanceamentos de classe.
*   **Insights Acionáveis:** Identificação dos principais fatores de risco de churn.
*   **(Futuro):** Simulação de impacto de ações de retenção.

## Tecnologias Utilizadas

*   **Linguagem:** Python 3.9+
*   **Bibliotecas Principais:**
    *   Pandas, NumPy: Manipulação e análise de dados.
    *   Scikit-learn: Modelagem, pré-processamento e avaliação.
    *   Matplotlib, Seaborn, Plotly (opcional): Visualização de dados.
    *   Jupyter Notebook: Análise exploratória e documentação.
*   **Gerenciamento de Ambiente:** venv / Conda

## Instalação e Configuração

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/DaniloBlancoMotta/Gym_Churn_Prediction.git
    cd Gym_Churn_Prediction
    ```

2.  **Crie um ambiente virtual:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/macOS
    # ou: venv\Scripts\activate  # Windows
    ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

#Como Usar

1.  **Dados:** Adicione os dados brutos da academia na pasta `data/raw/` (respeitando a privacidade e LGPD).
2.  **Análise:** Execute os notebooks em `notebooks/` para a análise exploratória.
3.  **Pipeline:** Execute o script principal (ex: `python src/main.py`) para pré-processar, treinar e avaliar o modelo.
4.  **Resultados:** Analise os relatórios e métricas gerados.

*(Nota: Este é um esqueleto de projeto. O código e os dados específicos precisam ser adicionados.)*

## 📊 Estrutura do Projeto

```
Gym_Churn_Prediction/
├── data/
│   ├── raw/          # Dados brutos (ex: historico_uso.csv, cadastro_clientes.csv)
│   └── processed/    # Dados limpos e preparados para modelagem
├── notebooks/        # Jupyter notebooks (EDA, experimentação)
│   └── 01_EDA_Gym_Churn.ipynb
├── src/              # Código fonte
│   ├── __init__.py
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   ├── evaluation.py
│   └── main.py       # Orquestrador do pipeline
├── requirements.txt  # Dependências
├── .gitignore
└── README.md

