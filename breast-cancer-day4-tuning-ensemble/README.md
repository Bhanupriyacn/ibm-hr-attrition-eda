# Day 4: Breast Cancer Classifier Tuning and Ensemble

This folder contains the Day 4 classifier tuning and ensemble notebook for the Kaggle Breast Cancer Wisconsin dataset:

https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data

## Deliverables

- `breast_cancer_tuning_ensemble_day4.ipynb`: notebook with baseline 5-fold CV, GridSearchCV, RandomizedSearchCV, and Random Forest ensemble.
- `breast_cancer_day4_results_table.csv`: single results table with model, CV accuracy, test accuracy, and best parameters.
- `submission-note.md`: short explanation of the selected model.

## Results Summary

| Model | CV Accuracy | Test Accuracy | Best Params |
| --- | ---: | ---: | --- |
| GridSearchCV Logistic Regression | 0.9758 | 0.9912 | `C=0.1`, `class_weight=balanced`, `penalty=l2`, `solver=liblinear` |
| RandomizedSearchCV Logistic Regression | 0.9758 | 0.9825 | randomized best Logistic Regression params |
| Random Forest Ensemble | 0.9604 | 0.9737 | `n_estimators=300`, `random_state=42` |
| Baseline Logistic Regression | 0.9736 | 0.9649 | default Logistic Regression |

## Selected Model

GridSearchCV Logistic Regression is selected because it achieved the highest test accuracy and tied for the strongest 5-fold CV accuracy while staying simpler than the ensemble model.
