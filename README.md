# Laptop Price Prediction: From Raw Text to Machine Learning

## Overview
This project involves building a complete machine learning pipeline to predict laptop prices based on their specifications. It covers everything from parsing unstructured text features and performing statistical analysis (ANOVA) to hyperparameter tuning and model evaluation.

## Key Features & Engineering
* **Feature Extraction & Encoding:** Parsed raw text columns (`Cpu`, `Gpu`) into distinct categorical features. Applied One-Hot Encoding (`pd.get_dummies`) to transform categorical variables into a feature matrix.
* **Data Type Optimization & Duplicates:** Converted string-based numerical fields to integers/floats and resolved hidden data duplication issues by applying transformations (`applymap` with `tuple`) to unhashable list types, dropping 28 duplicates.
* **Statistical Feature Selection:** Conducted one-way ANOVA tests to validate the statistical significance of categorical features in relation to price.
* **Machine Learning Pipeline:** Trained and evaluated multiple regression models including Linear Regression, Decision Tree, Random Forest, and XGBoost.
* **Hyperparameter Tuning:** Utilized `GridSearchCV` to optimize the XGBoost regressor, achieving a final R² score of 0.84.

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, SciPy

## Dataset
The dataset used in this project is the widely known "Laptop Price Prediction" dataset from Kaggle.
* **Source:** [Kaggle - Laptop Prices](https://www.kaggle.com/datasets/muhammetvarl/laptop-price)

## How to Explore
1. Clone the repository: `git clone https://github.com/myroslav284/laptop-price-prediciton.git`
2. Open the Jupyter Notebook `laptop_price.ipynb` directly on GitHub to view the executed code, data transformations, and model evaluations.
