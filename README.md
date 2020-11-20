# First Modeling Project - Ames Housing Data and Kaggle Challenge

Welcome to Project 2! It's time to start modeling.

### Overview

In the world of real estate and selling of property, there are multiple aspects of a house that determine the sale price. Some include but are not limited to the neighborhood, condition of the house, how big the house is, year built, etc. All of these aspects contribute some value to determine the sale price. 


### Problem Statement

A real estate agent who advertises a house wants to know which are the most important aspects to feature first on his/her advertisement online. There is a dataset provided what can help him/her with it. However, there are too many features to fit in one advertisement. Therefore, using linear regression models would be an ideal way to determine what should be listed in the advertisement. The goal is to build the best regression model One mandatory aspect that has to be on the advertisement has to be the neighborhood.

### Analysis Brief Summary

The first task that had to be done involved exploratory data analysis. From the data, we saw that many features were related to each other and conducted feature engineering where we added/multiplied several columns to create one feature. From there, various charts were created including scatterplots, a boxplot, and a heatmap. The boxplot helped identify the potential outliers of the dataset. The heatmap provided the list of correlations. The heatmap provided the potential variables that could be significant to the linear model. Lastly, the scatterplots provided the general trend between the variables with the highest correlation and what we are trying to predict which is the sale price of the property. 

From there, we created our linear regression model. This involved train-test splitted, scaled our data, and finally initiating the linear regression model. We also created regression models using LASSO and RIDGE.

We see that the R2 scores for the training and testing data are .88 and .86 respectively which indicate that the model is leaning towards not generalizing well to new data. This also indicates a higher variance or an overfit and lower bias.

The Root Mean Squared Error for the model is on the higher side, indicating that there are ways to improve our model including taking the log of the dataset features. 


### Recommendations/Downsides of the Linear Model

Based on the linear regrssion coefficents, we see that the neighborhoods that have the highest impact on our model include the e Bridge
North Ridge, and North Ridge Heights neighborhoods. 

The features that the real estate agent should list on top of the advertisement are the interior space, basement rating, and house condition.

Some of the limitations of this model is that perhaps some neighborhoods are left out of the linear model. Therefore the real estate agent would be limited to the amount of profits that he/she makes due to less advertisements generated from the linear model recommenations. Some potential ways to improve our linear model and advertising would include but not limited to: more neighborhoods and features.
