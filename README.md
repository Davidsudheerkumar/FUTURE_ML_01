# 📊 Sales & Demand Forecasting — FUTURE_ML_01

## 🔍 Objective

The objective of this project is to build a Sales & Demand Forecasting system using historical business data.

Sales forecasting helps businesses:

- Plan inventory efficiently  
- Manage staffing requirements  
- Optimize cash flow  
- Reduce overstocking and losses  
- Make proactive business decisions  

This project demonstrates how Machine Learning can support real business planning.

---
## 📁 Dataset Information

Dataset Used: Store Sales – Time Series Forecasting (Kaggle)

Files Used:
- train.csv → Historical daily sales data
- stores.csv → Store information
- items.csv → Product information

Target Variable:
- Sales (Daily Store Sales)

The dataset contains historical sales data used to predict future demand.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Google Colab  

---

## 🚀 Project Workflow

### 1️⃣ Business Understanding
Understanding how forecasting helps businesses make data-driven decisions.

### 2️⃣ Data Loading & Cleaning
- Loaded historical sales data  
- Converted date columns to datetime format  
- Checked for missing values  
- Aggregated total daily sales  

### 3️⃣ Time-Based Feature Engineering
Created features to capture trend and seasonality:

- Month  
- Day  
- Day of Week  
- Week of Year  
- Lag Features (previous day sales)  
- Rolling Average (7-day moving average)  

These features help the model learn temporal patterns.

### 4️⃣ Train-Test Split
Used a time-based split (80% training, 20% testing).

No random shuffling was applied to avoid data leakage.

## 🤖 Model Used

Model: Linear Regression

Reason:
Linear Regression was chosen to capture the overall sales trend over time.

Features Used:
- Time_Index (trend feature)

Target:
- Daily Sales

### 6️⃣ Model Evaluation

The model was evaluated using:

- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  

### 📊 Results

MAE: 90445.69  
RMSE: 136338.63  
MAPE: 34.67%

The model serves as a baseline forecasting approach. 
While it captures overall trend patterns, advanced models such as Random Forest or Gradient Boosting could further improve forecasting accuracy.
---

## 📈 Visualizations

The project includes:

- Total Daily Sales Trend  
- Monthly Seasonality Analysis  
- Actual vs Predicted Sales Plot  
- Forecast Visualization  

These visualizations make the results understandable for non-technical stakeholders.

---

## 🧠 Business Interpretation

The forecasting model identifies trends and seasonal patterns in historical sales data.

If predicted demand increases:
- Businesses can increase inventory
- Prepare additional staffing
- Ensure product availability

If predicted demand decreases:
- Businesses can reduce stock orders
- Optimize operational costs
- Avoid overproduction

This system helps businesses move from reactive decisions to proactive planning.

---

## 📁 Repository Structure

FUTURE_ML_01  
│  
├── Sales_Demand_Forecasting_FUTURE_ML_01.ipynb  
└── README.md  

---

## ▶ How to Run This Project

1. Download dataset from Kaggle  
2. Open the notebook in Google Colab  
3. Upload dataset files  
4. Run all cells sequentially  

---
## 🧹 Data Preprocessing

✔ Converted 'date' column to datetime format  
✔ Aggregated daily sales  
✔ Checked and handled missing values  
✔ Created time-based features (Year, Month, Day)  
✔ Created Time Index feature for trend modeling  
---

## ✅ Conclusion

This project demonstrates a complete Machine Learning workflow for business sales forecasting:

- Data Preparation  
- Feature Engineering  
- Model Training  
- Evaluation  
- Business Interpretation  

It provides a foundation for building more advanced forecasting systems using models such as Random Forest, XGBoost, or time-series specific approaches.
