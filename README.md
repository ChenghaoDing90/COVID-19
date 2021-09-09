# Covid19
A class project to predict Covid-19 affection numbers in county level of US.
## Project Description
This project uses county level data about demographics and health-related information to predict one week deaths from April 23rd to April 30th. We consider some predictor variables, such as the polulation, age distribution, gender distribution, per capita share of medical resources and health conditions. 

## Clustering
At first, to give a simple understanding, we perform the covid-19 growing pattern clustering by k-means method,
demographics clustering by spectral method and health-related information clustering by agglomerative
hierarchical clustering method. 

We find cases and health resource are highly affected by the economic situation of a county. Comparing to them, deaths and demographics do not show any obvious regional characteristics and scatter throughout the country. The classification performs well and can give identify most counties with high death rate.

## One Week Prediction
We use logistic regression and support vector machine to predict whether death per 100,000 population in the county is larger than 1. Then, four regression methods, elastic penalized regression, random forest regression, GAM regression and XGBoost method, are used to to predict one week deaths, based on the previous days’ amount of deaths, the cases a week ago and the characteristics of demogrphics and health-related information.

We conclude that the the population and population density makes their death toll rise even faster in the county. People over 85 with heart disease are more vulnerable to this virus. Comparing to male, female are more vulnerable. It is helpful for reducing the deaths to provide adequate medical resource, such as a hospital. However, because of the population base, age density and gender density are related to social situation in this area, we think the analysis of vulnerable poeple are affected.
