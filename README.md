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

Each row represents a property with both numerical and categorical attributes.

---

## 🎯 Objectives
- Data collection from Kaggle  
- Data cleaning and preprocessing  
- Feature selection and encoding  
- Data visualization and correlation analysis  
- Model training and testing  
- Model evaluation using regression metrics  
- Result interpretation and insights  

---

## ⚙️ Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Scikit-learn** | Data preprocessing, model training |
| **Jupyter Notebook** | Development environment |
| **NumPy** | Numerical computation |
| **Pandas** | Data manipulation |
| **Matplotlib & Seaborn** | Data visualization |

---

## 🔍 Workflow

### 1️⃣ Data Cleaning
- Checked dataset shape, columns, and statistical summary  
- Handled missing values and removed irrelevant data  

### 2️⃣ Data Preprocessing
- **Feature Selection:** Chose relevant columns  
- **Categorical Encoding:** Used OneHotEncoding for `city` and `district`  
- **Log Transformation:** Applied `np.log1p()` on `price_inr` to reduce skewness  
- **Correlation Analysis:** Visualized relationships between features and target  

![Correlation Heatmap](images/correlation_heatmap.png)

---

### 3️⃣ Model Training
- Split dataset: **80% training / 20% testing**  
- Trained **Linear Regression model** using `sklearn.linear_model.LinearRegression`  
- Extracted coefficients and intercept for interpretation  

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)
print("Coefficients:", model.coef_)
print("Intercept:", model.intercept_)
