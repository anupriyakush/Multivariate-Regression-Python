# Multivariate-Regression-Python

import statsmodels.api as sm
import xlrd
import pandas as pd
from sklearn.preprocessing import StandardScaler
scale = StandardScaler()
df = pd.read_excel('C:/Users/anupr/Documents/External Courses/Udemy - datascience/cars.xls')
print(df.head())
x = df[['Mileage','Cylinder','Doors']]
y = df['Price']
x = scale.fit_transform(x)
est = sm.OLS(y,x).fit()  #ordinary least square
print(est.summary())
