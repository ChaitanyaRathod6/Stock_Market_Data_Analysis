# Stock Market Data Analysis & Prediction

## Overview
This project focuses on analyzing stock market trends and building a predictive model for stock prices. Using historical data from Yahoo Finance, we explore market patterns, assess volatility, and apply machine learning techniques to forecast future stock prices.

## Dataset
- **Source:** Yahoo Finance
- **Includes:** Date, Open, High, Low, Close, Volume, Adjusted Close Prices
- **Data Quality:** No missing values found

## Project Workflow
### 1. Data Collection & Preprocessing
- Fetched historical stock prices using Yahoo Finance API
- Verified data integrity and handled any inconsistencies
- Created additional features like moving averages and lagged variables

### 2. Exploratory Data Analysis (EDA)
- Visualized stock price movements over time
- Examined moving averages (SMA, EMA) and volatility (Bollinger Bands)
- Analyzed correlations between stocks and compared performance with the S&P 500

### 3. Feature Engineering
- Introduced lagged features for past closing prices
- Computed short- and long-term moving averages
- Included stock volatility metrics

### 4. Machine Learning Model
#### Models Implemented:
- **Random Forest Regressor** (Baseline Model)
- **XGBoost Regressor** (Optimized for better performance)

#### Process:
1. Split the dataset into **training (80%) and testing (20%)**
2. Trained models on historical price data
3. Evaluated predictions using **Mean Absolute Error (MAE)**
4. Visualized predicted vs. actual stock prices

### 5. Results & Key Takeaways
- Random Forest provided a reasonable baseline but struggled with market fluctuations
- XGBoost offered improved predictions with lower error
- Further enhancements possible with deep learning models like LSTM

## Potential Improvements
- Implement **LSTM (Long Short-Term Memory)** for time-series forecasting
- Optimize hyperparameters for better model accuracy
- Develop a trading strategy based on model predictions

## Dependencies
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (Machine Learning)
- XGBoost
- Yahoo Finance API

## Running the Project
1. Install dependencies:  
   ```sh
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost yfinance
   ```
2. Run the script:
   ```sh
   python stock_analysis.py
   ```

## Conclusion
This project showcases the application of **data science and machine learning** in stock market analysis. While models provide valuable insights, financial markets are influenced by external factors, making absolute predictions challenging. The project serves as a foundation for further exploration and refinement.



