# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>we find multi varient linear regtrssion using pandas.

### Step2
<br>we find from sklearn import linear model.

### Step3
<br>First we have to read a file using pandas.

### Step4
<br>In this programm we take 2 variables weight and volume.

### Step5
<br>Using this two variables we find coefficient and intercept.

## Program:
```
###Developed by: Janani R
###Register number: 212221230039

import pandas as pd
from sklearn import linear_model

df =pd.read_csv("cars.xls")
x= df[["Weight","Volume"]]
y= df["CO2"]
regr =linear_model.LinearRegression()
regr.fit(x,y)

print("coefficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedco2=regr.predict([[3000,1200]])
print("Predicted co2 for the coressponding weight and volume ",predictedco2)

```
## Output:
![multivariate](./cars.png)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.