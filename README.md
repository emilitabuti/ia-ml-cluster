# IA ML Cluster - Clustering das receitas do orçamento dos EUA

Mini projeto de **IA não supervisionada** (disciplina de IA/ML). A ideia é agrupar contas de receita do orçamento federal americano que se comportam de forma parecida ao longo do tempo (1962-2015).

- Notebook com EDA e modelos: [eda_clustering_budget.ipynb](eda_clustering_budget.ipynb)
- Dados: `data/BUDGET-2016-DB-3.csv` (Public Budget Database, FY 2016, tabela de Receipts - [govinfo.gov](https://www.govinfo.gov/app/details/BUDGET-2016-DB/BUDGET-2016-DB-3))
- Modelos usados: K-Means (escolhido, k = 5), Affinity Propagation, Hierárquico (Ward) e DBSCAN

## Resultado resumido

| Modelo | Clusters | Silhueta |
|---|---|---|
| K-Means | 5 | 0,40 |
| Affinity Propagation | 5 | 0,40 |
| Hierárquico (Ward) | 5 | 0,38 |
| DBSCAN | 7 (+63 ruídos) | 0,51 (sem ruído) |

Os 5 grupos do K-Means: receitas grandes e permanentes, receitas novas, previdência (fora do orçamento), receitas encerradas e contas instáveis/de ajuste.

## Como rodar

```bash
pip install -r requirements.txt
jupyter notebook eda_clustering_budget.ipynb
```

## Integrantes

- Emili Vieira Tabuti
- (nome do colega)
