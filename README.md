# adult_income

# Adult Income Classification

A machine learning classification project using the Adult Census Income dataset to predict whether an individual's annual income is above or below $50K based on demographic, educational, and employment-related features.

## Problem Statement

The goal of this project is to predict whether a person's income is:

- `<=50K`
- `>50K`

This is a binary classification problem.

## Dataset

The dataset contains information such as:

- Age
- Workclass
- Education
- Marital Status
- Occupation
- Relationship
- Race
- Sex
- Capital Gain
- Capital Loss
- Hours per Week
- Native Country

The target variable is `income`.

## Data Preprocessing

The following preprocessing steps were performed:

- Handled missing/unknown values represented by `?`
- Converted the target variable into binary values:
  - `<=50K → 0`
  - `>50K → 1`
- Separated numerical and categorical features
- Applied One-Hot Encoding to categorical features
- Applied Yeo-Johnson transformation to `fnlwgt`
- Used `ColumnTransformer` and `Pipeline` for preprocessing and modeling

## Models Used

Two classification algorithms were implemented:

1. Logistic Regression
2. Decision Tree Classifier

## Evaluation

The models were evaluated using:

- Accuracy Score
- Cross-Validation Score

### Results

| Model | Test Accuracy | Cross-Validation Accuracy |
|---|---:|---:|
| Logistic Regression | 84.52% | 85.17% |
| Decision Tree | 81.27% | 81.38% |

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Conclusion

The project demonstrates an end-to-end machine learning workflow for binary classification, including exploratory data analysis, preprocessing, feature transformation, model training, cross-validation, and evaluation.
