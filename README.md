# Stock_Prediction

# ![istockphoto-1170740969-170x170](https://user-images.githubusercontent.com/74747022/142938598-dfc1e2c5-70eb-42b3-8f82-3aefae9be016.jpg)

## Project Overview
This repository is a project focused on developing a live stock analysis dashboard with build in machine learning functions.
The goal is to build a dashboard that is useful to stock traders and allows them to gain additional insight from machine learning.
After trying several models, I determined that the best model for the dashboard is an XGBOOST model. This is mostly due to its ease of use and speed. The dashboard has two built in ML models, one for next day close price and one for next hour close price. From this project, I have determined 3 actionable conclusions and further work on the project.

## Business Problem
Stock prices are a a very important metric because they represent the value of publicly traded companies in  the eyes of society. There is also a strong financial incentive to have a higher stock value for current shareholders because stocks can be liquidated into currency. Stock prices fluctuate based on the supply and demand of stocks associated with a particular company. If stock price can be predicted it could bring these business values:
#### - Increased confidence of return when investing in a company's stock
#### - Increase the confidence of current shareholders regarding stock's direction which can influence their decision to buy/sell your stock
#### - Determine key metrics that drive a stock price up or down
#### - Forecasting stock crashes will lead to the minimization of capital loss
 

## Business Understanding
Predicting stock prices is not an easy task especially regarding the number of variables that go into it. Knowing that a stock price fluctuates based on supply and demand tells me how I will move forward. If I can collect general public sentiment towards a stock, current market trends, and the stock's recent direction, then I am confident that I can predict a stock's price. I will make two types of models for individual stocks, one that predicts the end of day price and one that predicts the price in 1 hour.

## Data
All information regarding this data can be found at https://fmpcloud.io/

## Modeling
In total, I developed 3 models. An ARIMA model, and two XGBOOST models. (One for daily predictions and one for hourly predictions). 
### Model Comparisons
<img width="629" alt="Screen Shot 2021-11-22 at 2 10 41 PM" src="https://user-images.githubusercontent.com/74747022/142939554-43a36e26-abe1-4090-b15e-6b61529e0a44.png">
<img width="638" alt="Screen Shot 2021-11-22 at 2 45 05 PM" src="https://user-images.githubusercontent.com/74747022/142939640-05b619d4-34c5-4516-9a98-35646eefb9bf.png">


### ARIMA Model
<img width="422" alt="Screen Shot 2021-11-22 at 2 47 07 PM" src="https://user-images.githubusercontent.com/74747022/142939888-fad17117-81b2-4157-ad37-47e59c4444ee.png">

### Daily XGBOOST
<img width="981" alt="Screen Shot 2021-11-22 at 2 50 10 PM" src="https://user-images.githubusercontent.com/74747022/142940266-f6ab0bb7-5474-4a81-bbe2-5474cd621f0b.png">

### Hourly XGBOOST
<img width="995" alt="Screen Shot 2021-11-22 at 2 49 13 PM" src="https://user-images.githubusercontent.com/74747022/142940294-232dcbd8-bcd9-41f6-83a2-00187ffc68f2.png">

## Conclusions
 - News Sentiment adds value to stock prediction
<img width="905" alt="Screen Shot 2021-11-22 at 2 55 22 PM" src="https://user-images.githubusercontent.com/74747022/142940885-190dac2e-2291-442f-bdcb-3cb2c3d35c0c.png">

 - Arima model is too slow for a live dashboard implementation
 
 - Stock market volatiliy adds noise to prediction models. To mitigate this, reduce the test set size i.e. the more recent the train data the more accurate the model.


