# Previsão de Doença Cardíaca

Projeto de machine learning para prever a probabilidade de um paciente ter doença cardíaca, com base em dados clínicos e de estilo de vida.

## O que o notebook faz

1. Carrega e limpa o dataset (`data/heart_disease_dataset.csv`, 1000 registros).
2. Trata valores nulos e converte colunas categóricas (Yes/No, gênero, tipo de dor no peito) em variáveis numéricas via one-hot encoding.
3. Treina e compara vários modelos de classificação: Regressão Logística, Árvore de Decisão, Random Forest, Gradient Boosting, SVM, KNN e Naive Bayes.
4. Avalia os modelos por acurácia, precisão, recall, F1-Score e ROC-AUC, incluindo validação cruzada.
5. Conclui que o **Naive Bayes** é o melhor modelo para o problema, por ter bom equilíbrio entre detectar doentes (recall) e evitar falsos alarmes (precisão), sem sinais de overfitting.

## Como rodar

```bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook model_heart_disease.ipynb
```

> Certifique-se de que o dataset esteja em `data/heart_disease_dataset.csv`.

## Requisitos

Veja `requirements.txt`.
