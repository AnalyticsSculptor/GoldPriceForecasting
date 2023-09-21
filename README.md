# GoldPriceForecasting
Gold Price Forecasting Project 
The Gold Price Forecasting project aims to predict the future prices of gold based on historical daily price data and other related financial instruments. Gold is a precious metal widely recognized for its value and has been used as a form of investment and a safe-haven asset for centuries. The price of gold is influenced by various factors, including economic conditions, geopolitical events, inflation rates, and market sentiment. Accurate forecasting of gold prices is essential for investors, traders, and financial institutions to make informed decisions and manage risks effectively.

Dataset Information: The dataset for this project contains historical daily price data for various financial instruments, with a focus on gold-related features. The dataset includes features such as Open, High, Low, Close, Adjusted Close prices, and volume for gold (symbol: GLD) as well as other related financial instruments like the S&P 500 (SPY), Dow Jones (DJI), Euro Currency Index (EUR/USD), Oil (USO), and more. The time period covered by the dataset spans several years, making it suitable for time series analysis.

Objective: The primary objective of the Gold Price Forecasting project is to build a predictive model that can forecast the future prices of gold based on historical price
data and relevant financial indicators. The model will be trained on past price patterns and will aim to make accurate predictions about future price movements. By doing so, the project seeks to provide valuable insights to investors and traders to optimize their gold-related investment strategies and manage their risk exposure effectively.

Methodology:
1. Data Preprocessing: The initial step involves loading the dataset, converting the "Date" column to a datetime format for time series analysis, and computing the correlation of each feature with the "Adjusted Close" price. Features with low correlation will be dropped to focus on relevant ones.
2. Exploratory Data Analysis (EDA): Data visualization techniques will be employed to gain insights into the time series trends and relationships between different features. Line plots will be used to visualize the time series data for different features.
3. Time Series Split: The dataset will be split into training and testing sets using TimeSeriesSplit, a cross-validation technique designed for time series data.
4. Model Selection and Evaluation: The LightGBM Regressor, a powerful gradient boosting machine learning algorithm, will be chosen as the forecasting model. Cross-validation with repeated k-fold will be used to evaluate the model's performance.
5. Forecasting: The LightGBM model will be fitted to the training data to learn from past price patterns and relationships between features.
6. Model Evaluation: The model's performance will be assessed using evaluation metrics such as Mean Absolute Error (MAE) and R-Squared to measure its accuracy and goodness of fit.
7. Visualization: The actual vs. predicted values will be visualized using bar plots to provide a clear comparison and understanding of the model's forecasting capabilities.
