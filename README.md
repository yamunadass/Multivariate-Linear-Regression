# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas.
### Step2
Impor linear model from sklearn.
### Step3
Read the files cars.csv.
### Step4
Assign he values for x and y as requried.
### Step5
Create the LinearRegression model and predic he output
## Program:
```
Developed by:Yamuna M
RegisterNumber: 212223230248

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
```
## Output:
![image](https://github.com/yamunadass/Multivariate-Linear-Regression/assets/138971172/1e8c9596-d9fc-4d4a-b66a-d64d27671288)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
