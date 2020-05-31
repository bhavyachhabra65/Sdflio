# Sdflio
ML project on predictions on covid19

Objectives behind this project - 
Build an ML model for predicting the number of total infections in India till 31st of July 2020.
Build an ML model for predicting the number of deaths in India till 31st of July 2020.
Build an ML model and predict recovery rate and death rate in India for the period 15th June to 31st of July.


In this project, we have predicted the futuristic impact of Covid-19 in India with several measures of mistakes that organisations or citizens make. In this report we have used fbprophet, an inbuilt script from facebook. It implements a procedure for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. Prophet is robust to missing data and shifts in the trend, and typically handles outliers well.

We have assumed three levels in this project which are actually the mistakes done to handle Covid-19, from which level-1 is the slightest mistake and level-3 is the mistake which does have the biggest impact. So we prepared a formula using various measures. 

Impact ∝ Level
Impact ∝ Current cases

=>  Impact = k * (current cases) * (level) ** 2

=>  0.283 * current cases * level**2

By using this formula, we have calculated the predictions by multiplying the Impact with Predicted cases without Impact.

In this project, we have calculated the predictions using fbprophet. This module clearly defines the numbers to be achieved and shows us weekly and overall trends with upper and lower cuts. This module seems to be best fitted with the project we are working on.

