# 🧠 Product Sales Volume Prediction – GDGOC 2025

## 📘 Overview
This project was developed as part of the **Google Developer Group Open Competition (GDGOC) 2025**, focusing on predicting the **sales volume of a product** using historical data.  

The goal of this project is to build a machine learning model capable of estimating future product sales volumes based on features such as product type, price, marketing spend, store location, and seasonal trends.  

This project demonstrates a complete end-to-end data science workflow — from data cleaning, exploratory data analysis, feature engineering, and model training, to evaluation and interpretation — as a part of Group 9’s final GDGOC project.

---

## 📊 Dataset
- **Source:** Provided during GDGOC 2025 competition  
- **Total Samples:** ~10,000 records  
- **Main Features:**
  - `product_name` – type of product  
  - `category` – product category  
  - `price` – selling price  
  - `marketing_spend` – amount spent on promotion  
  - `store_location` – sales outlet region  
  - `month`, `year` – temporal features  
  - `sales_volume` – target variable (number of products sold)  

---

## ⚙️ Workflow

### 1. Exploratory Data Analysis (EDA)
- Analyzed distribution of product sales and feature relationships.  
- Detected correlations between marketing spend, price, and total sales.  
- Visualized seasonal sales trends across different months and product categories.

### 2. Data Preprocessing
- **Handling Missing Values:** Imputed missing values using `SimpleImputer`.  
- **Encoding:** Converted categorical columns using one-hot encoding.  
- **Scaling:** Standardized numerical features using `StandardScaler`.  
- **Feature Selection:** Removed irrelevant and low-variance columns.

### 3. Feature Engineering
- Created new features such as:
  - Average monthly sales per product
  - Price-to-sales ratio
  - Seasonal index features  
- Combined time-based variables to capture trends and seasonality.

### 4. Model Training
- Trained several regression models including:
  - `LinearRegression`
  - `RandomForestRegressor`
  - `XGradientBoostingRegressor`
- Performed hyperparameter tuning using cross-validation to select the best-performing model.

### 5. Model Evaluation
- Evaluation Metrics: **Mean Absolute Error (MAE)** and **R² Score**  
- Best model achieved:
  - **MAE:** ≈ : 0.3206 
  - **R² Score:** ≈ 0.82  
- Results showed the XGradientBoostingRegressor model produced the most stable predictions and lowest error.
