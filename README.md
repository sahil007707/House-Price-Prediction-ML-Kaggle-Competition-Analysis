# 🏡 House Price Prediction - Kaggle Competition


> 💡 Predicting final house sale prices using advanced data preprocessing, feature engineering, and machine learning for Kaggle competition success.

---

## 📦 Overview

This repository contains my complete solution for the **House Prices: Advanced Regression Techniques** Kaggle competition. The challenge is to predict the **final sale price of homes** in Ames, Iowa based on a rich set of features describing the properties.

I performed thorough **EDA, data cleaning, feature engineering, modeling, and evaluation**, ensuring robust predictions while following best practices for competitions.

---

## 📂 Files Included

| File Name                                             | Description                                   |
|-------------------------------------------------------|-----------------------------------------------|
| `train.csv`                                            | Original training data                        |
| `test.csv`                                             | Original test data                            |
| `House Price Prediction ML Kaggle Competition.ipynb`  | Full notebook with code and analysis          |
| `train_cleaned.csv`                                   | Cleaned training data after preprocessing     |
| `test_cleaned.csv`                                    | Cleaned test data ready for model prediction  |
| `submission.csv`                                      | Final predictions in Kaggle submission format |
| `README.md`                                            | Project documentation                         |

---

## 🔍 Exploratory Data Analysis (EDA)

- Identified and visualized **missing values**
- Detected and handled **skewed features**
- Analyzed relationships between features and `SalePrice`
- Outlier detection and removal using distribution plots and IQR

---

## 🧼 Data Cleaning & Preprocessing

- Dropped features with **>50% missing values**
- Imputed missing values using:
  - **Median** for numerical columns
  - **Mode** for categorical columns
- Converted categorical features using **Label Encoding**
- Scaled numerical features using `StandardScaler`

---

## 🏗️ Feature Engineering

- Created new features like:
  - `TotalSF` = Total Square Footage
  - `AgeOfHouse` = YrSold - YearBuilt
- Log-transformed `SalePrice` and skewed numeric columns
- Reduced multicollinearity using correlation analysis

---

## 🧠 Machine Learning Models

Tested multiple regression models:
- ✅ `XGBoost Regressor`
- ✅ `LGBMRegressor`
- ✅ `CatBoost Regressor`
- ✅ `Ridge` and `Lasso Regression`
- ✅ `RandomForestRegressor`

> 🔥 **Best Model**: XGBoost (lowest RMSE on cross-validation)

---

## 🧪 Evaluation

- Evaluation Metric: **Root Mean Squared Error (RMSE)**
- Used K-Fold Cross-Validation to ensure model robustness
- Created final `submission.csv` for Kaggle submission

---

## 📈 Final Results

| Model              | Public LB Score (RMSE) |
|-------------------|------------------------|
| XGBoost Regressor | 🥇 _Your best score_   |
| Lasso Regression  | _your score_           |
| LightGBM          | _your score_           |

> 🏁 _Final submission placed in top X% on leaderboard_ (update this as applicable)

---

## 🛠️ Tech Stack

| Purpose              | Tools/Libraries                     |
|----------------------|-------------------------------------|
| Language             | Python                              |
| Data Analysis        | pandas, numpy                       |
| Visualization        | seaborn, matplotlib, plotly         |
| Modeling             | scikit-learn, XGBoost, LightGBM     |
| Feature Engineering  | scipy.stats, sklearn.preprocessing  |

---

## 📌 How to Run

1. Clone the repository:
```bash
git clone https://github.com/sahil007707/house-price-kaggle.git
