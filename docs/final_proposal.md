# US Air Pollution Prediction and Forecasting using Machine Learning Models


### Introduction

Air pollution is one of the important environmental problems in metropolitan cities.Many air pollution indicators have an impact on people's health. Particulate matter (PM10), carbon monoxide (CO), and sulfur dioxide(so2) are a few of the significant indicators . Standards and guidelines for acceptable levels of these pollutants in the air have been established by the EU and other national environmental authorities. Short-term and long-term issues with human health may arise when the concentration levels of certain indicators surpass the air quality recommendations.

The air pollution forecasting system is a web-based system that collects meteorological data and data on air pollution from relevant web sites, anticipates air pollutant levels for the immediate future, and posts the results on a website.

### Why this project

One of the largest difficulties facing the globe today is air pollution, which also magnifies pre-existing medical conditions and causes respiratory, cardiovascular, and lung diseases. The health of the world may also be damaged. Therefore, it becomes crucial to lessen air pollution and raise awareness of these issues.

It is simpler to control and reduce the dangers of air pollution and ensure a safe level of pollutant concentration in the area with an accurate approach of air pollution forecasting. Additionally, it assists in evaluating the hazards that poor air quality regulations provide to the environment and the climate. Planning daily activities more easily, avoiding places with high alert levels, and putting appropriate pollution control measures into place are all benefits of accurate forecasting.


### Questions to answer

1.which state has highest air pollution.

2.which Model is best for prediction.

3.Analysing the future air pollution quality in U.S.

4.which pollutant has high effect in air quality index.



### Dataset

it is difficult to forecast the wolrdwide air pollution,so i have choosen u.s air pollution for forecasting.


data source link:https://data.world/data-society/us-air-pollution-data

This dataset contains data of air pollution of diiferent states in u.s

this dataset has 147679 rows × 29 columns

it is a time series data. this dataset has data from 2000-01-01 to 2010-06-06.

This dataset deals with pollution in the U.S. Pollution in the U.S. has been well documented by the U.S. EPA.

Includes four major pollutants (Nitrogen Dioxide, Sulphur Dioxide, Carbon Monoxide and Ozone).
 
columns in this dataset are:

State Code : The code allocated by US EPA to each state

County code : The code of counties in a specific state allocated by US EPA

Site Num : The site number in a specific county allocated by US EPA

Address: Address of the monitoring site

State : State of monitoring site

County : County of monitoring site

City : City of the monitoring site

Date Local : Date of monitoring

The four pollutants (NO2, O3, SO2 and O3) each has 5 specific columns. For instance, for NO2:

NO2 Units : The units measured for NO2

NO2 Mean : The arithmetic mean of concentration of NO2 within a given day

NO2 AQI : The calculated air quality index of NO2 within a given day

NO2 1st Max Value : The maximum value obtained for NO2 concentration in a given day

NO2 1st Max Hour : The hour when the maximum NO2 concentration was recorded in a given day

### Models 
There are many methods for forecasting the data.In this project i am using some popular ML models like 

1.linear regression

2.logistic regression

3.decission tree regression

4.random forest regression

5.MA model 

6.AR model

7.ARIMA


for forecasting the future air quality index.I want to compare these models by calculating the RMSE value and want to pick the best model out of these models for predicting the future air quality index.


### Expectations
To find the best machine learning model for prediction based on the RMSE value and To forecast the air quality.


### Reference:
https://www.kaggle.com/datasets/sogun3/uspollution
