# Project 2: Predicting Housing Prices with Linear Regression

## Introduction & Problem Statement

The main objectives of the project are followings:

To apply data preprocessing and preparation techniques in order to obtain clean data.
To build machine learning models to predict house price base on the house features
To analyse and compare models performance and choose the best model
Modelling algorithm is used to build an optimise predictive model to predict the housing price. RMSLE and coefficient determination R2 are used to evaluate the model. Ridge, Lasso and Linear regression will be used for regularize the model.

Most of the variables are exactly the type of information that a typical home buyer would want to know about a potential property ( (e.g. When was it built? How big is the lot? How many square feet of living space is in the dwelling? Is the basement finished? How many bathrooms are there?).

The model is expected to be used to help a home buyer (primary stakeholder) to obtain the proper price by adjust their bid price accordingly. Also, property owners (Secondary stakeholder) may find the model useful to post a reasonable sale price of their home in the property market.l should react to unseen sets of data without large variations in accuracy. Ultimately, I'll be looking to evaluate the performance of this model using root mean squared error (RMSE) or the measure of the differences between values predicted by the model and the values observed.

## Summary 
Lasso model was the most successful in predicting housing sale prices. On the dataset comprising of 30% of the test data, the model achieved an RMSE of 22390. On the dataset comprising of the other 70% of the test data, the model performed within expectations, returning an RMSE of 22217. It also has a high R2 on our training data, where it can explain up to 93.4% of the variance in sale price.

## Recommendations
Based on our model, the homeowner :

- Improve on Overall Condition, Overall Quality, 1st Floor Area and Ground Living Area, since these are continuous variables.
- Expand Basement Finished Area only if the house is situated on flat land (Land Contour)
- Expand Masonry Veneer Area only if the house is situated on flat land (Land Contour)
- If the house is in neighborhood D, reduce the areas of Basement Finished, Total Basement and Masonry Veneer
- Minimise the Basement areas
- Sell the house while it is still young

For homebuyers:

- Buy houses with good Overall Condition, Overall Quality, and large 1st Floor Area and Ground Living Area
- If the house is situated on flat land, buy houses with small or no Basement Finished Area and Masonry Veneer Area, so that you can increase these aspects later on
- If the house is in neighborhood D, avoid those with Basement Finished, Total Basement and Masonry Veneer Areas
- Buy houses with small or no Basement areas
- Buy houses which are young, since prices deteriorate with age

## Data Dictionary
A detailed data dictionary can be found [here](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).