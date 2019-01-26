# Multivariate-Regression-Python
Used multivariate regression to analyze which covariate is the best predictor of the response variable 'Price'


In the dataset we have a price column, that represents the price that each vehicle sold for, the mileage of that vehicle, the make, model, trims, and body type,number of cylinders and litres of the engine,number of doors and some binary data of whether it has cruise control, sound system, or leather.
We are trying to find out the most influential covariate to predict the car prices. I used Ordinary Least Square model using the statsmodel package.  I called fit to create the model based on the features in X and the value in Y(Price).
It turns out that the number of cylinders is actually the most prominent feature of this model with the highest absolute value coefficient. 
