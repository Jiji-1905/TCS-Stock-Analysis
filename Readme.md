# 📈 TCS Stock Price Analysis & Prediction

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-orange)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Data%20Visualization-red)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-purple)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-yellow)
![RandomForest](https://img.shields.io/badge/Model-Random%20Forest-darkgreen)
![LinearRegression](https://img.shields.io/badge/Model-Linear%20Regression-lightgrey)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

# 📌 Project Overview

This project analyzes historical stock price data of **Tata Consultancy Services (TCS)** and builds machine learning models to predict stock closing prices using historical market indicators.

The project demonstrates a complete **Data Analyst workflow**, including:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Machine Learning Modeling
- Model Evaluation
- Model Saving for Future Use

The goal is to identify patterns in stock price movements and build predictive models based on historical stock data.

---

# 📊 Dataset Information

The dataset contains historical stock price data with the following columns:

| Column | Description |
|------|-------------|
| Date | Trading date |
| Open | Opening stock price |
| High | Highest stock price |
| Low | Lowest stock price |
| Close | Closing stock price |
| Volume | Trading volume |

---

# ⚙️ Technologies Used

| Tool | Purpose |
|-----|--------|
| Python | Programming Language |
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-Learn | Machine learning models |

---

# 🔎 Data Preprocessing

Steps performed in preprocessing:

- Converted **Date column to datetime format**
- Sorted dataset by date
- Converted numerical columns to numeric format
- Handled missing values using **forward fill method**
- Checked dataset statistics and structure

---

# 📊 Exploratory Data Analysis

## Stock Closing Price Trend

This visualization shows the trend of **TCS closing stock price over time**.

![Close Price](outputs/close_price_over_time.png)

---

## Moving Average Analysis

Two moving averages were calculated:

- **50-Day Moving Average**
- **200-Day Moving Average**

These indicators help identify **short-term and long-term market trends**.

![Moving Average](outputs/moving_average.png)

---

# 🧠 Feature Engineering

New features extracted from the date column:

| Feature | Description |
|------|-------------|
| Year | Trading year |
| Month | Trading month |
| Day | Day of month |
| Day_of_Week | Day of the week |
| Prev_Close | Previous day's closing price |

These features help machine learning models understand **temporal stock market patterns**.

---

# 🤖 Machine Learning Models

Two machine learning models were implemented:

## 1. Random Forest Regressor

Random Forest is an ensemble learning algorithm that builds multiple decision trees and combines them to improve prediction accuracy.

Advantages:

- Handles complex patterns
- Reduces overfitting
- Works well with financial data

---

## 2. Linear Regression

Linear Regression models the linear relationship between independent variables and the target variable.

Used to:

- Compare performance with Random Forest
- Provide a baseline model

---

# 📉 Model Evaluation

Model performance was evaluated using:

| Metric | Description |
|------|-------------|
| Mean Squared Error (MSE) | Measures prediction error |
| R² Score | Measures model performance |

Higher **R² score** indicates better prediction performance.

---

# 📊 Prediction Visualization

The following chart compares **Actual vs Predicted stock prices**.

![Prediction](outputs/actual-vs_predicted_values.png)

---

# 💾 Model Saving

The trained model is saved using **Pickle** for future predictions.

```
TCS_Stock_Predictor.pkl
```

This allows the model to be reused without retraining.

---

# 📁 Project Structure

```
tcs_stock_analysis
│
├── csv_files
│   ├── TCS_stock_history.xlsx
│   └── TCS_stock_history.csv
│
├── outputs
│   ├── close_price_over_time.png
│   ├── moving_average.png
│   └── actual-vs_predicted_values.png
│
├── TCS_Stock_Predictor.pkl
├── tcs_stock_analysis.ipynb
└── README.md
```

---

# 🚀 Key Insights

Important findings from the analysis:

- Stock prices follow clear long-term trends.
- Moving averages help identify market momentum.
- Previous closing price strongly influences future price.
- Random Forest model captures nonlinear patterns effectively.

---
# Google Colab : https://colab.research.google.com/drive/1IGJSx6yzVZ6eJg4aPQzp4iaTXWLU5rdJ?usp=sharing

# 📌 Future Improvements

Possible enhancements for this project:

- Add **LSTM deep learning model for time series prediction**
- Include **technical indicators (RSI, MACD, Bollinger Bands)**
- Build an **interactive dashboard using Streamlit or Power BI**
- Deploy the model for real-time prediction

---

# 👨‍💻 Author

**Jiji Babu**

Aspiring Data Analyst

Skills:

- Python
- SQL
- Data Analysis
- Machine Learning
- Data Visualization

---

