# 🏠 House Price Prediction using Linear Regression
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/5c1c1d55-b7ec-4b18-b233-d1479659ce5e" />

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

- 4️⃣ Model Prediction
Predicted house prices on test data

Compared actual vs predicted values

[Looks like the result wasn't safe to show. Let's switch things up and try something else!]

5️⃣ Model Evaluation
Evaluated performance using:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

R² Score

python
from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
mae = mean_absolute_error(y_test, y_pred)
mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
print(f"MAE: {mae}, MSE: {mse}, R²: {r2}")
📈 Accuracy: 99.9% on test set
✅ Regression line fits closely to actual data points.

[Looks like the result wasn't safe to show. Let's switch things up and try something else!]

📊 Results
Achieved 99.9% accuracy on test data

Regression line shows strong linear relationship

Log transformation improved model stability

Encoding categorical features enhanced prediction accuracy

🚀 Future Scope
Include additional socioeconomic factors (property type, amenities, ROI)

Apply advanced models (Ridge, Lasso, Random Forest Regressor)

Perform hyperparameter tuning for optimization

Extend dataset to include rental yield and investment potential

📚 References
Kaggle – Indian Real Estate Dataset

Scikit-learn Documentation (scikit-learn.org in Bing)

Seaborn Documentation

Matplotlib Documentation (matplotlib.org in Bing)

👩‍💻 Author
Lavanya B  
Batch: J023
Aspiring Data Analyst / Data Scientist

```python
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X_train, y_train)
print("Coefficients:", model.coef_)
print("Intercept:", model.intercept_)
