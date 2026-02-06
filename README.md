# TATASTEEL-OHLC-PREDICTION-
 This project provides a machine learning pipeline to predict the next-day Open, High, Low, and Close (OHLC) stock prices of Tata Steel based on 20 years of historical NSE data. The model leverages time-series features and multi-output regression techniques to forecast price movements and support data-driven investment insights
# Tata Steel OHLC Price Prediction 

**Predicting next-day Open, High, Low, Close (OHLC) stock prices using Machine Learning**

---

## Project Overview
This project focuses on forecasting the **next-day OHLC prices** of Tata Steel using **20 years of historical NSE stock data**. Daily stock prices are highly volatile and influenced by multiple factors like market trends, buying/selling pressure, and news events. This repository demonstrates a complete machine learning workflow from **data preprocessing to prediction deployment**, aimed at providing data-driven insights for stock analysis.

---

## Key Features

- **Data Cleaning & Preprocessing:**  
  - Handles missing values and inconsistent columns  
  - Converts numeric columns with commas to proper numeric types  
  - Extracts year, month, and day from the Date column

- **Feature Engineering:**  
  - Selects relevant features for predicting next-day OHLC  
  - Drops redundant or non-informative columns  

- **Multi-Output Regression:**  
  - Supports **Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting**  
  - Predicts multiple outputs (Open, High, Low, Close) simultaneously  

- **Model Evaluation:**  
  - Performance metrics: **R², RMSE, MAPE**  
  - Train-test evaluation and unseen data validation  

- **Streamlit Deployment Ready:**  
  - Interactive web application for live OHLC predictions  
  - Easily deployable for internal testing or portfolio analysis  

- **Trained Model Persistence:**  
  - Model saved using **Pickle** for quick inference on new data  

---

## Dataset

- Collected from **NSE (National Stock Exchange of India)**  
- Daily historical stock data spanning ~20 years  
- Key Features:  
  - `Date`, `Symbol`, `Series`, `Prev Close`, `Open`, `High`, `Low`, `Last`, `Close`, `VWAP`, `Volume`, `Turnover`, `Trades`, `Deliverable Volume`, `%Deliverable`  

---

## Folder Structure


---

## Getting Started

1. **Clone the repository**

```bash
git clone https://github.com/ashok8601/TATASTEEL-OHLC-PREDICTION.git
cd TATASTEEL-OHLC-PREDICTION

pip install -r requirements.txt

streamlit run app.py

import pickle
with open("models/TATASTEEL.pkl", "rb") as f:
    model = pickle.load(f)
predicted_ohlc = model.predict(new_data)



## Evaluation Metrics
Metric
Train Score
Test Score
R²
0.99
0.92
RMSE
4
16
MAPE
0.01
0.01
High R² on training and strong generalization on unseen data demonstrates model robustness.



## Technologies Used
Python 3.x
Pandas, NumPy – Data manipulation
Scikit-learn – Regression & MultiOutput Regression
Streamlit – Web deployment


## Outcome
A complete ML workflow to predict Tata Steel’s next-day OHLC stock prices. The project is ready for:
Data-driven analysis and investment insights
Streamlit-based interactive visualization
Integration into trading dashboards

Author
Ashok Kumar – B.Tech CSE | Data Science & ML Enthusiast
GitHub�
LinkedIn�
