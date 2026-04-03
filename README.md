# Walmart_Sales_Forecasting

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange)
![Machine Learning](https://img.shields.io/badge/Focus-Regression-green)

## 📌 Project Overview
This project was developed as part of my Data Science training. The goal is to build a machine learning model capable of estimating weekly sales in Walmart stores with high precision. 

By analyzing historical sales data alongside economic indicators (CPI, Unemployment, Fuel Price), this model helps understand how external factors influence retail performance and assists in planning future marketing campaigns.

## 🎯 Project Goals
The analysis is divided into three main phases:
1.  **Exploratory Data Analysis (EDA) & Preprocessing**: Cleaning data, handling missing values, removing outliers (3rd sigma rule), and feature engineering on dates.
2.  **Baseline Modeling**: Training a simple Linear Regression to establish a reference performance.
3.  **Regularization**: Implementing Ridge and Lasso regression to fight overfitting and improve generalization.

## 📊 Dataset & Features
The dataset contains information about weekly sales from several Walmart stores.
* **Target Variable**: `Weekly_Sales`
* **Numerical Features**: Temperature, Fuel_Price, CPI, Unemployment, Year, Month, Day, DayOfWeek.
* **Categorical Features**: Store ID, Holiday_Flag.

## 🚀 Key Results
The transition from a simple linear model to a regularized model (Ridge) allowed for better stability and performance on unseen data.

| Model | R² Score (Train) | R² Score (Test) | Status |
| :--- | :---: | :---: | :--- |
| Linear Regression | 0.987 | 0.935 | Overfitting detected |
| **Ridge Regression (α=0.01)** | **0.981** | **0.953** | **Best Model** |

## 💡 Main Insights
* **Store Location**: The specific Store ID is the most significant predictor of sales volume.
* **CPI (Inflation)**: Showed a strong positive correlation with sales value in this specific dataset.
* **Seasonality**: Feature engineering on dates (Month/Day) was crucial to capture sales trends.

## 🛠️ Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/walmart-sales-forecasting.git](https://github.com/YOUR_USERNAME/walmart-sales-forecasting.git)
