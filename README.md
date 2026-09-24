# Capstone-AIM-AI-and-Machine-Learning-2026-Jefferson-Capistrano
This is part of my AI and Machine learning that I enrolled at AIM
# Machine Learning-Based Fraud Detection for Financial Transactions

## Project Overview

This capstone project develops an end-to-end machine learning solution
for detecting fraudulent credit card transactions.

The dataset contains 284,807 transactions with 492 fraud cases,
representing approximately 0.17% of the original dataset.

The project covers data preprocessing, exploratory data analysis,
feature engineering, feature selection, dimensionality reduction,
machine learning model development, model evaluation, explainability,
bias and fairness considerations, and deployment considerations.

## Business Problem

Financial institutions must detect fraudulent transactions while
minimizing disruption to legitimate customers.

Because fraud is extremely rare, accuracy alone is not an appropriate
measure of model quality. PR-AUC was therefore selected as the primary
evaluation metric, supported by precision, recall, F1 score, ROC-AUC
and confusion-matrix analysis.

## Models Evaluated

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- Regularized XGBoost experiment

## Model Performance

| Model | Precision | Recall | F1 | ROC-AUC | PR-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.0552 | 0.8737 | 0.1039 | 0.9686 | 0.6704 |
| Decision Tree | 0.2284 | 0.7789 | 0.3532 | 0.8887 | 0.5378 |
| Random Forest | 0.9324 | 0.7263 | 0.8166 | 0.9473 | 0.8051 |
| XGBoost | 0.8462 | 0.8105 | 0.8280 | 0.9752 | 0.8151 |
| Regularized XGBoost | 0.1298 | 0.8526 | 0.2253 | 0.9793 | 0.6733 |

## Selected Model

XGBoost was selected as the champion model because it achieved the
highest test PR-AUC (0.8151), which was defined as the primary metric
before model comparison.

The model achieved:

- Precision: 84.62%
- Recall: 81.05%
- F1 Score: 82.80%
- ROC-AUC: 97.52%
- PR-AUC: 81.51%

## Explainability

SHAP was used to analyze global feature importance. The most influential
features included V14, V4, V12, V10 and V11.

Because V1-V28 are anonymized PCA-derived variables, their effects can
be interpreted statistically but cannot be mapped directly to specific
customer or transaction characteristics.

## Repository Structure

- `notebooks/` - Complete Google Colab/Jupyter notebook
- `src/` - Reusable preprocessing, training and evaluation scripts
- `data/` - Dataset documentation and source information
- `models/` - Model artifact documentation
- `reports/` - Final capstone report
- `presentations/` - Technical and business presentations

## Reproducibility

Random seed: 42

The notebook contains the complete workflow from dataset loading through
model evaluation and explainability.

## Author

Jefferson Capistrano

Capstone Project – Artificial Intelligence and Machine Learning
