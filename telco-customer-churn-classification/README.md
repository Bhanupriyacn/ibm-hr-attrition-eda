# Telco Customer Churn Classification

This folder contains a classification notebook for the Kaggle Telco Customer Churn dataset:

https://www.kaggle.com/datasets/blastchar/telco-customer-churn

## Deliverables

- `telco_customer_churn_classification.ipynb`: notebook with Logistic Regression, Decision Tree, Random Forest, and KNN classifiers.
- `telco_churn_metrics_comparison.csv`: metrics comparison table.

## Best Model

The selected model is Random Forest because it produced the highest F1-score on the held-out test set while keeping churn recall strong.

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
| --- | ---: | ---: | ---: | ---: | ---: |
| Random Forest | 0.765 | 0.544 | 0.727 | 0.622 | 0.831 |
| Decision Tree | 0.736 | 0.503 | 0.794 | 0.616 | 0.828 |
| Logistic Regression | 0.726 | 0.490 | 0.797 | 0.607 | 0.835 |
| KNN | 0.776 | 0.582 | 0.559 | 0.570 | 0.816 |

Best-model confusion matrix:

```text
[[805, 228],
 [102, 272]]
```

## Run

Open the notebook in Jupyter, Google Colab, or Kaggle. The notebook can load the dataset from an attached Kaggle dataset, a local `data/` folder, or through `kagglehub`.
