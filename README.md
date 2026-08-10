# 🏠 House Price Prediction using Linear Regression
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5c1c1d55-b7ec-4b18-b233-d1479659ce5e" />

# 🏠 House Price Prediction using Linear Regression

## 📌 Project Overview
This project focuses on predicting **house prices in the Indian real estate market** using **Linear Regression**.  
The dataset captures property listings from major cities — Chennai, Mumbai, Delhi, Bangalore, Hyderabad, and Pune — with attributes such as area, number of rooms, location, and age of the house.

The goal is to build a regression model that accurately estimates property prices based on these features.

---

## 🧾 Dataset
- **Source:** Kaggle – *Indian Real Estate Market Dataset*  
- **Target Variable:** `price_inr` (Property Selling Price)  
- **Features Used:**
  - `built_up_area_sqft`
  - `bedrooms`
  - `bathrooms`
  - `age_years`
  - `city`
  - `district`
  - `price_inr`

---

## 🎯 Objectives
- Collect dataset from Kaggle  
- Perform **data cleaning** and **preprocessing**  
- Apply **feature selection** and **encoding**  
- Visualize correlations and distributions  
- Train and test the Linear Regression model  
- Predict house prices for unseen data  
- Evaluate model performance using metrics  

---

## 🛠️ Tools & Technologies
- **Scikit-learn** → Data Preprocessing & Model Training  
- **Jupyter Notebook** → Development Environment  
- **NumPy** → Numerical Computation  
- **Pandas** → Data Manipulation  
- **Matplotlib & Seaborn** → Data Visualization  

---

## 🔎 Data Preparation
### 1. Data Cleaning
- Checked dataset shape, columns, and statistical summary  
- Handled missing values and removed irrelevant data  

### 2. Preprocessing
- **Feature Selection** → Selected meaningful features  
- **Categorical Encoding** → Applied OneHotEncoding for `city` and `district`  
- **Log Transformation** → Applied `np.log1p(price_inr)` to reduce skewness  
- **Correlation Analysis** → Visualized feature correlations using heatmaps  

---

## 📊 Model Training & Prediction
- **Train-Test Split:** 80% training, 20% testing  
- Fitted Linear Regression model on training data  
- Predicted house prices on test set  
- Extracted model coefficients and intercept  

---

## 📈 Model Evaluation
- **Metrics Used:**
  - Mean Absolute Error (MAE)  
  - Mean Squared Error (MSE)  
  - R² Score  

- **Results:**
  - Achieved **99.9% accuracy** on test set  
  - Visualized regression line with scatter plot (Actual vs Predicted Prices)  

---

## ✅ Results & Conclusion
- Successfully built a Linear Regression model for house price prediction  
- Learned the importance of **data cleaning, preprocessing, encoding, and evaluation**  
- Achieved high accuracy with strong regression line fit  
- Hands-on experience from raw data collection to actionable insights  

---

## 🔮 Future Scope
- Analyze **socioeconomic factors** (city, district, property type) for regional trends  
- Study **financial variables** like price per sqft for investment potential  
- Evaluate **feature importance** to improve forecasting accuracy  

---

## 📚 References
- Kaggle – *Indian Real Estate Dataset*  
- Scikit-learn Documentation – Model Training & Evaluation  
- Seaborn & Matplotlib Documentation – Data Visualization  

---

## 👩‍💻 Author
**Lavanya B**  
Aspiring Data Analyst / Data Scientist



