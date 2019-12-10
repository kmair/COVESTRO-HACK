# COVESTRO Hackathon 

This Hackathon was held in September 2019 and this analysis is carried out for Rhine Water Level Predictions. This prediction would help
COVESTRO to: 
- Avoid shortage of raw materials.
-	Efficient distribution of finished goods, reducing inventory buildup and customer dissatisfaction.
-	Effective use of water in the production process. 

An overview of the problem can be found [here](https://github.com/kmair/COVESTRO-HACK/blob/master/RhineWaterLevelUseCaseOverview.docx). 
This `.docx` file provides the problem statement.

Following the analysis this [Poster](https://github.com/kmair/COVESTRO-HACK/tree/master/Poster) created summarizes all the findings.

## Summary of all the Analysis

**1. Exploratory Data Analysis.ipynb**

A preliminary data analysis was carried out. There are multiple weather stations but predictions have to be carried out only at Duesseldorf 
and Cologne. For weather information, the closest weather station data was assigned. An additional parameter of `incoming water` was 
calculated for these river stations by checking the nodes.

**2. ARIMA modeling of features**

For each quarter year, data is provided for 3.5 months following which predictions for the next 3 days has to be carried out. Thus, to 
model on these features, an ARIMA model was used to fill the values of the variables.

**3. Regression models**

This looks at fitting Gradient Boosting Regressor, Random Forest Regressor, Bayes Ridge Regression, Passive Aggressive Regressor
TheilSenRegressor, and Linear regression models for predicting the water level. 

![Regression models overview](https://github.com/kmair/COVESTRO-HACK/blob/master/Poster/Images/Regression%20output.PNG)

**4. NN_model**

For improving the model, a machine learning algorithm was implemented.
