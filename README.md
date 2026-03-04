# Credit Risk Analytics

![License](https://img.shields.io/github/license/burgerman/credit_risk_modelling)
![Repo Size](https://img.shields.io/github/repo-size/burgerman/credit_risk_modelling)
![Last Commit](https://img.shields.io/github/last-commit/burgerman/credit_risk_modelling)

## Overview

This project provides a comprehensive end-to-end analysis and modeling pipeline for credit risk assessment. Using a loan default dataset, the project demonstrates advanced data science techniques to predict creditworthiness, including robust feature engineering, statistical significance testing, and state-of-the-art machine learning models.

The primary analysis is contained within the [Credit_Risk_Analytics.ipynb](Credit_Risk_Analytics.ipynb) notebook.

---

## Key Features

- **Exploratory Data Analysis (EDA)**: Detailed visualization of feature distributions and their relationships with loan defaults.
- **Statistical Analysis**: Implementation of ANOVA (F-test) for numeric features and Chi-square tests for categorical features to identify predictive power.
- **Outlier Detection**: Usage of Median Absolute Deviation (MAD) via the `PyOD` library for robust outlier identification.
- **Advanced Feature Engineering**:
    *   **Binning**: Transform continuous variables into meaningful categorical bins (DTI, Mortgage Due, File Age, etc.).
    *   **Missing Value Handling**: Systematic treatment of null values using indicators and categorical grouping.
    *   **WOE & IV**: Calculation of Weight of Evidence (WOE) and Information Value (IV) for credit scorecard development.
- **Machine Learning**: Implementation of gradient boosting frameworks including **XGBoost** and **LightGBM**.
- **Hyperparameter Optimization**: Automated tuning using **Optuna**.
- **Model Interpretability**: Integration of **SHAP** values to explain model predictions and feature importance.

---

## Project Workflow

1.  **Environment Setup**: Installation of specialized libraries (`pyod`, `optuna`, `shap`).
2.  **Data Preprocessing**: Converting currency strings to numeric values and handling data types.
3.  **EDA & Visualization**: Analyzing default rates across occupations, loan reasons, and financial ratios.
4.  **Feature Selection**: Using statistical tests and correlation matrices to refine the feature set.
5.  **Feature Engineering**: Implementing binning strategies and missingness indicators.
6.  **Model Training**: Training ensemble models with stratified cross-validation.
7.  **Evaluation**: Validating performance using ROC-AUC, Precision-Recall, and Kolmogorov-Smirnov (KS) statistics.

---

## Technologies Used

- **Languages**: Python
- **Data Analysis**: Pandas, NumPy, SciPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-Learn, XGBoost, LightGBM
- **Optimization**: Optuna
- **Interpretability**: SHAP
- **Outlier Detection**: PyOD

---

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook or Google Colab

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/burgerman/credit_risk_modelling.git
   cd credit_risk_modelling
   ```

2. Install the required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn xgboost lightgbm optuna shap pyod
   ```

3. Run the analysis:
   Open `Credit_Risk_Analytics.ipynb` in your preferred Jupyter environment.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

## Contact

Maintainer: [burgerman](https://github.com/burgerman)
