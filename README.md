# Medical Insurance Cost Prediction

## Overview
This project explores medical insurance cost prediction using exploratory data analysis (EDA) and machine learning models, including **Linear Regression** and **Random Forest Regressor**. The dataset (`insurance.csv`) contains demographic and health-related attributes, which are analyzed to determine key cost factors.

Steps in the analysis include:
- Exploratory Data Analysis (EDA) to visualize charge distribution and correlations
- Feature encoding and engineering for model training
- Model comparison between Linear Regression and Random Forest to identify the best predictor

---

## Dataset
The dataset used in this project is sourced from Kaggle: [Medical Cost Personal Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance).

---

## Exploratory Data Analysis (EDA)
EDA is performed using **Seaborn** and **Matplotlib** to:
- Visualize distribution of insurance charges, both raw and log-transformed
- Analyze correlations between smoking, age, BMI, and charges using a heatmap
- Compare cost distributions between smokers and non-smokers
- Study insurance costs across different age groups

---

## Feature Engineering
- Categorical variables (`sex`, `smoker`, `region`) are **label-encoded** using `LabelEncoder()`.
- `Age_Group` is created for grouping individuals (`18-29`, `30-44`, `45-59`, `60+`).
- **Standardization** is applied to numeric features before training models.

---

## Machine Learning Models
Two regression models are implemented:

### 1. Linear Regression
- Computes the best-fit line for predicting insurance costs

### 2. Random Forest Regressor
- Ensemble-based approach with multiple decision trees
- Captures **non-linear relationships** and provides feature importance scores

---

## Results & Insights
- **Smoking is the most significant factor** influencing insurance costs
- **Random Forest outperforms Linear Regression**, capturing non-linear patterns better
- **BMI and Age impact insurance charges**, but smoking leads to the steepest increase
- **Gender, number of children, and region** have minimal impact
