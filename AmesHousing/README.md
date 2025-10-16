# 🏠 Ames Housing Price Prediction

📖 Project Overview  
This project predicts **house sale prices in Ames, Iowa** using the **Ames Housing dataset**, a modern alternative to the classic Boston Housing dataset.  
It’s a full end-to-end data science workflow — from data cleaning and feature engineering to exploratory data analysis (EDA) and machine learning modeling.  

The dataset includes over 80 attributes describing residential properties, enabling rich exploration and regression modeling.

---

🎯 Objectives  
- Clean and preprocess raw housing data (handle missing values, outliers, and irrelevant columns)  
- Perform Exploratory Data Analysis (EDA) to identify trends and relationships with sale price  
- Engineer new features to improve model accuracy  
- Train and evaluate multiple regression models (Linear, Ridge and Random Forest)  
- Tune hyperparameters and compare performance metrics  
- Visualize residuals and error metrics for model interpretability  

📊 Methodology  

### 1. Data Cleaning  
- Removed unnecessary columns (`Order`, `PID`)  
- Handled missing values and encoded categorical quality metrics 
- Saved the cleaned dataset to `AmesHousing/data/processed/amesHousingCleaned.csv`

### 2. Exploratory Data Analysis (EDA)  
- Explored distributions, correlations and key relationships  
- Identified most influential features correlated with `SalePrice`  

### 3. Feature Engineering  
- Combined and aggregated key attributes:  
  - `Total Bathrooms` (sum of full and half baths)  
  - `Overall Qual Gr Liv` (interaction of overall quality × living area)  
  - `Built Decade` (bucketed construction year)  
- Saved engineered dataset as `AmesHousing/data/processed/amesHousingFeatureEngineering.csv`

### 4. Machine Learning  
Models used:
- **Linear Regression** – baseline model  
- **Ridge Regression (RidgeCV)** – regularized regression with best α selected via cross-validation  
- **Random Forest Regressor** – non-linear model with grid search optimization  

Training, hyperparameter tuning and evaluation are handled in `AmesHousing/src/ameshousingml.py`.

### 5. Evaluation Metrics  
Performance is assessed using:
- Mean Absolute Error (MAE)  
- R² Score  
- Mean Absolute Percentage Error (MAPE)  

📂 Dataset  
- **Name:** Ames Housing Dataset  
- **Source:** [Kaggle - Ames Housing Data](https://www.kaggle.com/datasets/prevek18/ames-housing-dataset)  
- **Description:** 2,930 observations and 82 features describing residential homes in Ames, Iowa.
