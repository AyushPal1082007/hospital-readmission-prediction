# Hospital Readmission Prediction

## Overview

This project predicts whether a patient will be readmitted to the hospital within 30 days using Logistic Regression with L2 regularization.

## Objective

The objective is to develop a binary classification model that estimates 30-day hospital readmission risk from patient and hospital-related features.

## Dataset

The dataset contains 32,300 patient records with information including:

* Age
* Length of hospital stay
* Number of diagnoses
* Number of medications
* Previous admissions
* Glucose level
* BMI
* Diabetes status
* Discharge type

The target variable is:

`readmitted_30days`

where:

* `0` = No readmission within 30 days
* `1` = Readmission within 30 days

## Methodology

The project follows these steps:

1. Data loading
2. Data inspection
3. Data cleaning
4. Missing-value handling
5. Exploratory data analysis
6. Train-test split
7. Feature scaling
8. Logistic Regression with L2 regularization
9. Prediction
10. ROC-AUC evaluation
11. Confusion matrix analysis
12. Clinical cost analysis

## Machine Learning Model

Logistic Regression was selected as the classification algorithm.

L2 regularization was applied to help control model complexity and reduce the effect of excessively large coefficients.

## Evaluation

The primary evaluation metric is ROC-AUC.

Additional evaluation metrics include:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix

## Clinical Considerations

False negatives can be clinically important because a patient who is actually at high risk of readmission may not receive additional intervention.

False positives may result in unnecessary use of healthcare resources.

Therefore, the appropriate classification threshold should consider the relative clinical costs of false negatives and false positives.

## Tools and Technologies

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* GitHub

## Project Structure

```text
hospital-readmission-prediction/
│
├── Hospital_Readmission_Prediction.ipynb
└── README.md
```
