
# US Air Pollution Prediction and Forecasting using Machine Learning Models


#### ppt link:https://github.com/DATA-606-SPRING-2023-TUE/pragathi_data_606-1/blob/main/docs/Capstone.pptx

#### you tube video link:https://youtu.be/fEPTsuvnjW8


# Contents
1.Objective

2.Introduction

3.Dataset

4.Data Cleaning

5.Data Visualization

6.Machine Learning Models

7.Comparision Of Models

8.Forecasting

9.Conclusion



# 1.Objective
The objective of this project is to provide accurate and timely information on the levels of air pollutants in a united states, typically over the next 10 days.

The main goals of this project are:

To inform the public about the air quality in their area and alert them to potential health risks associated with exposure to pollutants.

To help policymakers make informed decisions about air quality regulations and mitigation strategies.

To assist industries and businesses in managing their emissions and complying with air quality regulations.

To provide early warnings to vulnerable populations, such as those with respiratory illnesses or the elderly, so that they can take steps to protect their health.

One of the largest difficulties facing the globe today is air pollution, which also magnifies pre-existing medical conditions and causes respiratory, cardiovascular, and lung diseases. The health of the world may also be damaged. Therefore, it becomes crucial to lessen air pollution and raise awareness of these issues.

It is simpler to control and reduce the dangers of air pollution and ensure a safe level of pollutant concentration in the area with an accurate approach of air pollution forecasting. Additionally, it assists in evaluating the hazards that poor air quality regulations provide to the environment and the climate. Planning daily activities more easily, avoiding places with high alert levels, and putting appropriate pollution control measures into place are all benefits of accurate forecasting.



# 2.Introduction
Air pollution refers to the presence of harmful substances in the air we breathe. These substances, known as pollutants, can be natural or man-made, and they can have serious negative effects on human health, the environment, and the economy.

Common sources of air pollution include industrial activities, transportation, power generation, and household activities like cooking and heating. Pollutants can take the form of gases, such as carbon monoxide and sulfur dioxide, or particulate matter like dust and soot.

The effects of air pollution can be seen and felt in many different ways. For example, exposure to air pollution can cause respiratory problems, heart disease, and cancer. It can also damage crops and forests, harm wildlife, and contribute to climate change.

Efforts to reduce air pollution are ongoing, and involve a combination of regulation, technology development, and public education. Governments around the world have established air quality standards, and many companies and individuals are taking steps to reduce their emissions.

In this project, I'm using the U.S. Air Quality Index dataset to analyze the air pollution in various U.S. states and forecast the highly polluted state's future air quality index using machine learning models.



# 3.Dataset
This dataset contains data of air pollution of diiferent states in u.s

this dataset has 147679 rows × 29 columns

it is a time series data. this dataset has data from 2000-01-01 to 2010-06-06.

Includes four major pollutants (Nitrogen Dioxide, Sulphur Dioxide, Carbon Monoxide and Ozone).

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


Source: Data.world

https://data.world/data-society/us-air-pollution-data



# 4.Data Cleaning
I have used only few columns like 'State','Date Local','NO2 AQI','NO2 Mean','O3 AQI','O3 Mean','CO AQI','CO Mean','SO2 AQI','SO2 Mean'.

<img width="554" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/56bc212b-3c8e-4405-be6e-0a4d56255159">


My dataset has few null values

<img width="131" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/866e6392-3aab-44a1-9607-facadced1230">

Filled the null values using forward fill and backward fill methods

<img width="96" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/ef6322f9-aaaa-49b7-a2e5-90aba70deda8">


Dataset has repeated columns,so i deleted the repeated columns by keeping the first non-repeated values.


Calculated the overall Air Quality Index value based on the given values.Overall AQI is the maximum value of the AQI among the given pollutants.



# 5.Data Visualization
The graph showing the NO2 Air Quality Index level in different states in the U.S

<img width="295" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/141e1a1d-570d-4a3a-8e18-b64eaa595433">


The graph showing the SO2 Air Quality Index level in different states in the U.S

<img width="294" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/1ceef4d1-d8ea-4a33-afe9-cdf28675ee33">


The graph showing the CO Air Quality Index level in different states in the U.S

<img width="275" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/00ee0d98-ca14-4827-9466-f6e1747be1ca">


The graph showing the O3 Air Quality Index level in different states in the U.S

<img width="269" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/1737d1d3-1bdd-4248-8663-ebeaa87ef4b8">


From all the above graphs it is observed that California State has high AQI of all the four pollutants.So,for my further analysis i am considering only California State.

<img width="600" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/241fd839-396a-4168-9c62-3d68914d6d36">

This is final dataset i am using to apply machine learning models.



# 6.Machine Learning Models

There are many methods for forecasting the data.In this project i am using some popular ML models like

#### Regression Models
regression analysis is a set of statistical processes for estimating the relationships between a dependent variable and one or more independent variables 

1.linear regression: It is a linear approach for modelling the relationship between a scalar response and one or more explanatory variables (also known as dependent and independent variables). The case of one explanatory variable is called simple linear regression; for more than one, the process is called multiple linear regression.

2.logistic regression:the logistic model (or logit model) is a statistical model that models the probability of an event taking place by having the log-odds for the event be a linear combination of one or more independent variables.

3.decission tree regression:It is a supervised learning approach used in statistics, data mining and machine learning. In this formalism, a classification or regression decision tree is used as a predictive model to draw conclusions about a set of observations.

4.random forest regression:It is a supervised learning algorithm that uses ensemble learning method for regression. Ensemble learning method is a technique that combines predictions from multiple machine learning algorithms to make a more accurate prediction than a single model.

#### Time Series Models
ARIMA:ARIMA models are generally denoted as ARIMA (p,d,q)  where p is the order of autoregressive model, d is the degree of differencing, and q is the order of moving-average model.

p value is obtained by taking the optimum lag value from partial auto correlation function.

q value is obtained by taking the optimum lag value from auto correlation function.

5.MA model

6.AR model

7.ARIMA


# 7.Comparision Of Models
comparing all the machine learning models by considering Root Mean Square Error value(RMSE).Low the RMSE value it indicates the best model.

<img width="673" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/1aebe254-0f4c-43fb-a0e8-cfa25c7f25e2">

From the above regression models it is observed that Random Forest has less RMSE value,it indicates that Random Forest is the best model for prediction compared to other models.

<img width="673" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/806ab5a3-b8cc-4721-a244-548ce40f835c">

From the above time series models it is observed that Moving Average has less RMSE value,it indicates that Moving Average is best for forecasting the future values compared to other models.



# 8.Forecasting

<img width="156" alt="image" src="https://github.com/vunnampragathi/pragathi_data_606/assets/112585191/9918cd12-e486-409a-8da7-77ac0e3664ac">

Forecasted Air Quality Index values of california state for next 10 days using moving average model


# 9.Conclusion

From the above findings it is observed that,

i)california has highest air pollution

ii)Random Forest is the best model for prediction in Regression models

iii)Moving Average is the best model for prediction in Time Series Models

iv)Forecasted the next 10 days Air Quality Index of California





