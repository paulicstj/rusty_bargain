# 🚗 Rusty Bargain – Car Price Prediction with Machine Learning

## 🔍 Project Functionality  
**Rusty Bargain**, a used car sales service, is building an app that helps users estimate the **market value of their car** based on historical data and technical specifications. The project goal is to develop a machine learning model that can accurately predict car prices, while also evaluating the **trade-offs between prediction quality, training time, and inference speed**.

## 🛠️ Technologies and Methods  
- **Python** (Pandas, NumPy, Scikit-learn, LightGBM, CatBoost, XGBoost, Matplotlib, Seaborn)
- **Exploratory Data Analysis (EDA)**:
  - Boxplots to detect outliers in price  
  - Correlation matrix to identify key features affecting price
- **Baseline sanity check**: Linear Regression  
- **Model training and tuning**:
  - **Random Forest** with hyperparameter tuning  
  - **LightGBM** – tested for speed and accuracy  
  - **CatBoost** and **XGBoost** – evaluated for performance  
  - **Stochastic Gradient Descent (SGD)** – tested for speed benchmark  
- **Evaluation Metrics**:
  - **R² score** (coefficient of determination)  
  - **RMSE** (Root Mean Squared Error)  
  - **Training and prediction times**

## 📈 Key Findings and Conclusion  
- **LightGBM** was the best model overall, with:
  - **R² = 0.8031**, **RMSE = 1539.60**
  - **Training time: 2.49 sec**, **Prediction time: 0.40 sec**
- **Random Forest** achieved slightly better accuracy but required:
  - **Training time: 314.32 sec**, **Prediction time: 2.49 sec**
- **SGD** was the fastest but underperformed:
  - **R² = 0.4093**, **RMSE = 2666.91**

✅ **Conclusion**: **LightGBM** is the ideal model for this use case. It combines **high accuracy** with **fast training and inference**, making it suitable for **real-time applications** in Rusty Bargain's mobile app.

