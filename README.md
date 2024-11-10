# Introduction to Store Sales Forecasting

In today's competitive retail landscape, accurately predicting future sales is crucial for businesses to make informed decisions, optimize resources, and maintain a competitive edge. Store Sales Forecasting leverages historical data, statistical methods, and machine learning models to estimate future sales. This approach helps retailers and decision-makers anticipate **customer demand, manage inventory levels, and create effective sales and marketing strategies**.




# What is Store Sales Forecasting?

Store Sales Forecasting involves predicting the revenue or sales volume for individual stores or across retail networks over a specific time period. By using **historical sales data** and considering **external factors, such as holidays, events, economic trends, economy,and weather patterns**, forecasting models can project future sales patterns. These forecasts can range from short-term predictions (daily or weekly sales) to long-term forecasts (monthly or yearly sales), helping businesses strategically plan their operations.

## Challenges in Store Sales Forecasting

- **Trend** : Sales changes with respect to time, trend is defined as the rate of change
- **Seasonality** :  Many products experience seasonal fluctuations, making it necessary for models to account for time-based patterns.
- **External Influences**: Events like holidays, economic conditions, local events, and weather can significantly impact sales and must be factored into forecasts.
- **Store-Specific Variability**: Each store may have unique characteristics (seasonality and trend) due to the location and customer demographics that influence sales, making it essential to tailor forecasts for individual stores

**Ecquador economy depends upon the oil. So, it's necessary to kepp oil prices in account**

## Datasets

- Store Sales Forecasting : https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data

## Approach

### Data cleaning

- Data cleaning helps to judge the quality of data, while data cleaning we can check and fill empty values, check shape, find that are related to each other.

### EDA

- During **EDA**, I tried to study sales of different family, stores, seasonality, trend, and effect of external factors that effect sales.

### Data Engineering

- As per the **EDA** findings, I have created features like **seasonality**, **trend**, **lags**, **time features**.

### Model Selection

- I have selected **XGBoost Model** due to its readiness to handle complex datasets.

### Model Evalution

- I have create three XGBoost models with three different approaches and calculated their effectiveness using **RMSLE, R square**.
  1. **First Approach** - I have used data without any transformation.
  2. **Second Approach** - I have removed outliers
  3. **Third Approach** - I have used log transformation on dependent variable. Log transformations helps to find the non linear relationship between the variables.
 
## Result

- I have used Third Model because of the better performance than others, calculated using **RMSLE, R square**.
