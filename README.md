# 📈 Stock Price Prediction

## Predicting Future Stock Prices Using Historical Data

---

## 📌 Objective
The goal of this project is to predict future stock prices using historical stock data.  
Key objectives include:  
- Understanding stock price trends and patterns.  
- Building predictive models using historical features like Open, High, Low, Close, Volume, and engineered features.  
- Evaluating model performance and providing actionable insights.

---

## 📌 Approach
1. **Data Collection:**  
   - Selected Apple Inc. (AAPL) stock using `yfinance`.  
   - Collected historical daily data (Open, High, Low, Close, Volume) from 2015–2025.

2. **Data Preprocessing:**  
   - Handled missing values.  
   - Feature engineering: moving averages, exponential moving averages, daily returns, volatility, lag features.  
   - Scaling with `MinMaxScaler`.  
   - Chronological train-test split (80%-20%).

3. **Exploratory Data Analysis (EDA):**  
   - Visualized trends in Close price, daily returns, and volatility.  
   - Analyzed feature correlations and patterns.

4. **Model Selection & Training:**  
   - Baseline: Linear Regression, Random Forest.  
   - Advanced: LSTM sequences prepared for sequential prediction.  
   - Trained models and compared performance.

5. **Model Evaluation:**  
   - Metrics: RMSE, MAE, MAPE.  
   - Linear Regression outperformed Random Forest.  
   - LSTM sequences ready for modeling temporal dependencies.

6. **Reporting & Insights:**  
   - Key trends: upward trend in stock prices, varying volatility, small daily returns.  
   - Features like previous day prices, moving averages, and volatility are strong predictors.  
   - Limitations: Models may fail during sudden market shocks; predictions best for short-term.

---

## 📌 Key Insights
- **Linear Regression:** Best short-term predictions, very low error (RMSE=0.00321, MAPE=0.36%).  
- **Random Forest:** Poor performance on test set (RMSE=0.12633, MAPE=10.10%).  
- **LSTM:** Sequence data prepared to potentially capture long-term temporal dependencies.  
- Visualizations show actual vs predicted prices and error patterns, confirming Linear Regression reliability.

---

## 📌 Reproducibility
- Data fetched via `yfinance`.  
- Preprocessing steps, feature engineering, scaling, and train-test splits are included.  
- All model training and evaluation code is provided in the Jupyter Notebook.  

- ## Author
- Rimsha Iram
- [Check Portfolio](https://www.datascienceportfol.io/rimshairamanalytics)
- Let’s connect on [LinkedIn](https://www.linkedin.com/in/rimsha-iram-analytics)


---
tlib seaborn scikit-learn yfinance tensorflow
