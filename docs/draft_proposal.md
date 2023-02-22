# LOS ANGEL city Web traffic forecasting using time series

### Introduction
Since more and more people throughout the world have access to the internet recently, an increase in website traffic is probably unavoidable. The organization that is able to deal with the changes in traffic in the most effective way will succeed. The growth in website traffic has the potential to generate a lot of problems.

The quantity of sessions in a particular period of time is known as web traffic, and it varies greatly depending on the time of day, day of the week, and other factors. The amount of web traffic a platform can handle is determined by the size of the servers that host the platform.We don't want this to occur, but if there is more traffic than the servers can handle, the website may display this 404 error. The guests will leave as a result of that.


### Why this project
One of the most difficult issues in the field has always been predicting the future values of time series. A real-time dashboard has graphics that are constantly updated with the most recent information available. These data visualizations include a combination of historical data and current information that is helpful for spotting new trends and keeping track of productivity. Data that is time-sensitive is typically included in real-time dashboards.


### Questions to answer
1.which webpage has high traffic.

2.which Model is best for prediction.

3.Analysing the future traffic of the webpage.



### Dataset
The dataset contains the page and the number of visits to that page on a particular data.(145063, 551)

the dataset has 145063 rows and 551 columns.

The data has all floating type data.

It is a time series data.Data ranges from 2015-07-01 to 2016-12-31


### Models 
There are many methods for forecasting the data.In this project i am using some popular ML models like 

1.AR model

2.MA model 

3.LSTM

4.ARIMA

5.exponential smoothing

for forecasting the future website traffic.I want to compare these models by calculating the RMSE value and want to pick the best model out of these models for predicting the future website traffic.


### Expectations
To find the best machine learning model for prediction based on the RMSE value and To forecast the webpage traffic for a particular webpage.


### Reference:
https://medium.com/@jyshao53/web-traffic-time-series-prediction-using-arima-lstm-7ef3911845ae
