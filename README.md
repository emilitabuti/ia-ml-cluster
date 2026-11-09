# IA ML Cluster - Clustering das agências do orçamento dos EUA

Mini projeto de **IA não supervisionada** (disciplina de IA/ML). A ideia é agrupar as agências do governo federal americano que tiveram um comportamento de orçamento parecido entre 1976 e 2016.

- Notebook com EDA e modelo: [eda_clustering_budget.ipynb](eda_clustering_budget.ipynb)
- Dados: `data/budget.csv`, do Kaggle [US Federal Government Budget 1976-2022](https://www.kaggle.com/datasets/mfaaris/usa-budget-authority-by-agency-19762022)
- Modelo usado: **K-Means** (k = 5, silhueta 0,32)

## Resultado resumido

Os 5 grupos do K-Means: agências grandes e estáveis, médias de crescimento acelerado, médias de crescimento lento, pequenas e irregulares, e uma agência isolada (Executive Office of the President, por causa dos picos).

## Como rodar

```bash
pip install -r requirements.txt
jupyter notebook eda_clustering_budget.ipynb
```

## Integrantes

- Emili Vieira Tabuti
- Caroline Guimarães Campos
