# Laptop Price EDA & Data Preprocessing

## Overview
This project focuses on cleaning, preprocessing, and exploring a dataset of laptop specifications and prices. The primary goal is to transform raw, unstructured text data into a clean, machine-learning-ready format, followed by Exploratory Data Analysis (EDA) to uncover pricing trends.

## Key Features & Engineering
* **Feature Extraction:** Developed custom functions to parse raw text columns (`Cpu`, `Gpu`) and extract meaningful categorical and numerical features (e.g., Company, Type, Frequency).
* **Data Type Optimization:** Cleaned string-based numerical columns (`Ram` removing 'GB', `Weight` removing 'kg') and converted them to appropriate `int` and `float` types.
* **Complex Duplicate Handling:** Resolved hidden data duplication issues. Applied custom transformations (`applymap` with `tuple`) to handle unhashable list types generated during feature extraction, successfully identifying and dropping 28 duplicate records.
* **Exploratory Data Analysis:** Built a correlation matrix and visualized hardware distributions to identify key drivers of laptop prices.

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Matplotlib, Seaborn

## Dataset
The dataset used in this project contains 1,303 initial records with 15 features including RAM, CPU, GPU, Weight, Screen Resolution, and Price.
* **Source:** [Kaggle - Laptop Prices Dataset]([https://www.kaggle.com/datasets/ionaskel/laptop-prices](https://www.kaggle.com/datasets/muhammetvarl/laptop-price))

## How to Run
1. Clone the repository: `git clone https://github.com/your-username/laptop-price-eda.git`
2. Install dependencies: `pip install pandas matplotlib seaborn`
3. Download the `laptop_price.csv` file from the Kaggle link above and place it in the root directory of the project.
4. Run the Jupyter Notebook `laptop_price.ipynb` to explore the step-by-step preprocessing and analysis.
