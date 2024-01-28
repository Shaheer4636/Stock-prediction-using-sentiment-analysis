# Project - Sentiment Analysis of Twitter Data for Predicting Apple Inc. (AAPL) Stock Movement
## Project Description
This project involves analyzing Twitter data related to Apple Inc. and predicting its future stock trend using sentiment classification. The goal is to explore the correlation between social media sentiment and market trends, focusing on Twitter's real-time information on societal opinions and trends.

### Data Preprocessing
#### 1. Twitter Data:
Data from Kaggle covering the period from January 01, 2016, to August 31, 2019, was used for sentiment analysis.
Processed to include only data for days when the stock market was open (approximately 252 trading days per year).

#### 2. Stock Data:
Daily Apple stock data for the same period was collected from Yahoo Finance.
Adjusted closing prices were used for analysis, considering the stock split on August 31, 2020.
Data Integration:

#### 3. Merged Twitter data and daily stock prices to create a final CSV file for predictive analyses.
Model Training and Evaluation

#### 4. Two approaches were employed for analyses:
   
#### a) Classification:
Twitter polarity scores classified tweets into positive, negative, and neutral sentiments.
Apple stock prices were converted into binary values (0 and 1) based on the trend.
Algorithms used: Random Forest Classifier and Gradient Boosting Classifier.

#### b) Regression:
Twitter polarity scores, Twitter volume, and adjusted closing prices were used to predict future stock prices.
Random Forest Regressor, LSTM RNN, and XGBoost Regressor were used for analysis.
Results/Key Findings

#### Approach 1: Classification
Random Forest Classifier: Accuracy scores around 50-55%, indicating limited confidence in correlating stock movement with Twitter sentiments.
Gradient Boosting Classifier: Similar accuracy range, suggesting challenges in using sentiment analysis for stock prediction.

#### Approach 2: Regression
Random Forest Regressor: RMSE: 0.0993 | R-squared: 82.27%
LSTM RNN: RMSE: 0.1334 | R-squared: 68.01%
XGBoost Regressor: RMSE: 0.0477 | R-squared: 95.92%
Regression models showed more favorable results, with XGBoost Regressor performing optimally for simulating future prices.

### Enhanced Results
For both Random Forest Regression and Random Forest Classifier, we improved accuracy to Root Mean Squared Error: 0.052 approx and R-squared: 95.15%. This enhancement of approximately 30% resulted in a better fit for the values, showcasing improved predictive capabilities.

#### Limitations/Improvements
Limited Twitter data from Kaggle and a relatively short timeframe for analysis.
Integration of additional sentiment sources, such as NewsAPI headlines, could enhance the analysis.

