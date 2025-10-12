# 🌍 OpenAQ Air Quality Prediction

## 📖 Project Overview
This project leverages **OpenAQ's global air quality dataset** to analyze and predict pollutant concentration levels across various countries.  
Unlike simpler, pre-cleaned datasets, this project involves working with **raw, multi-country environmental data** containing irregularities, missing values and mixed data formats.

The goal is to build a **machine learning model** that predicts air pollutant concentration (`value`) based on factors such as pollutant type, geography, time and unit of measurement.  
It demonstrates an **end-to-end workflow**: from data ingestion and cleaning to model training, evaluation and saving.

---

## 🎯 Objectives
- Clean and preprocess raw OpenAQ air quality data:
  - Handle missing coordinates, inconsistent pollutant names and encoding issues
- Perform feature engineering:
  - Extract temporal features (year, month, day, hour, weekday)
  - Create derived flags (`is_weekend`, seasonal indicators)
- Train multiple regression models to predict air pollution concentration (`value`)
- Compare model performance (Random Forest, Ridge, SVM)
- Visualize model residuals and metric comparisons
- Save the best-performing model for future use

---
