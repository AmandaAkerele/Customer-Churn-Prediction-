# Customer-Churn-Prediction: Ecommerce



# Machine Learning Model Evaluation Report

## Introduction

Introduction
This report presents a comprehensive evaluation of various machine learning models applied to a dataset with a focus on addressing class imbalance for churn prediction in the Ecommer industry. The goal is to compare the performance of different models using resampling techniques and assess their ability to classify the target variable accurately.

Dataset
The dataset used for this analysis contains [brief description of the dataset, its size, and relevant features].

Models and Resampling Techniques
Four different machine learning models were evaluated:

Logistic Regression
Random Forest
Decision Tree
XGBoost

To mitigate the effects of class imbalance, two resampling techniques were applied:

SMOTE (Synthetic Minority Over-sampling Technique)
ADASYN (Adaptive Synthetic Sampling)
Evaluation Metrics
The models were evaluated using the following metrics:

Precision: The ratio of correctly predicted positive observations to the total predicted positives.
Recall: The ratio of correctly predicted positive observations to the all observations in actual class.
F1-Score: The weighted average of precision and recall.
AUC-ROC: The area under the receiver operating characteristic curve.

## Dataset Description

The dataset contains features and corresponding labels, where the positive class is significantly underrepresented. This class imbalance can lead to biased model performance.

## Resampling Techniques

To mitigate the class imbalance, two resampling techniques were applied: Synthetic Minority Over-sampling Technique (SMOTE) and Adaptive Synthetic Sampling (ADASYN). These techniques create synthetic instances of the minority class to balance the class distribution.

## Models Evaluated

The following classification algorithms were evaluated:

1. **Logistic Regression**
2. **Random Forest**
3. **Decision Tree**
4. **XGBoost**

## Evaluation Metrics

The models were evaluated using the following metrics on a test set:

- **Precision**: Ability to correctly classify positive instances.
- **Recall**: Proportion of actual positive instances correctly classified.
- **F1-score**: Harmonic mean of precision and recall.
- **AUC-ROC**: Area Under the Receiver Operating Characteristic curve.

## Model Evaluation Results

### Logistic Regression

- **SMOTE**: Precision = 0.44, Recall = 0.84, F1-score = 0.58, AUC-ROC = 0.89.
- **ADASYN**: Precision = 0.43, Recall = 0.84, F1-score = 0.57, AUC-ROC = 0.89.

### Random Forest

- **SMOTE**: Precision = 0.86, Recall = 0.88, F1-score = 0.87, AUC-ROC = 0.99.
- **ADASYN**: Precision = 0.84, Recall = 0.85, F1-score = 0.85, AUC-ROC = 0.98.

### Decision Tree

- **SMOTE**: Precision = 0.67, Recall = 0.85, F1-score = 0.75, AUC-ROC = 0.91.
- **ADASYN**: Precision = 0.69, Recall = 0.79, F1-score = 0.74, AUC-ROC = 0.93.

### XGBoost

- **SMOTE**: Precision = 0.84, Recall = 0.85, F1-score = 0.85, AUC-ROC = 0.98.
- **ADASYN**: Precision = 0.88, Recall = 0.89, F1-score = 0.89, AUC-ROC = 0.98.

## Model Comparison

A comparison of the models' performance metrics is summarized below:

| Model               | Resample | Precision | Recall | F1-score | AUC-ROC |
|---------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | SMOTE    | 0.44      | 0.84   | 0.58     | 0.89    |
| Logistic Regression | ADASYN   | 0.43      | 0.84   | 0.57     | 0.89    |
| Random Forest       | SMOTE    | 0.86      | 0.88   | 0.87     | 0.99    |
| Random Forest       | ADASYN   | 0.84      | 0.85   | 0.85     | 0.98    |
| Decision Tree       | SMOTE    | 0.67      | 0.85   | 0.75     | 0.91    |
| Decision Tree       | ADASYN   | 0.69      | 0.79   | 0.74     | 0.93    |
| XGBoost             | SMOTE    | 0.84      | 0.85   | 0.85     | 0.98    |
| XGBoost             | ADASYN   | 0.88      | 0.89   | 0.89     | 0.98    |

## Conclusion

The evaluation shows that XGBoost with the ADASYN resampling technique consistently performs well across various metrics. It effectively addresses class imbalance and yields high AUC-ROC scores. This suggests that XGBoost with ADASYN is a strong candidate for further refinement and deployment in real-world scenarios.

## Recommendations

- Further hyperparameter tuning can be performed to optimize model performance.
- Additional feature engineering might enhance model robustness.
- Consider evaluating the models on external datasets to validate generalization.

## Acknowledgments

This analysis was conducted using Python with the support of popular libraries including scikit-learn and XGBoost.

---
*Date of Report: [April 2023]*
