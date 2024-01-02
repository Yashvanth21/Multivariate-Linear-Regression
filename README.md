# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Read the csv file.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3

## Program:
```
#To write a python program to implement multivariate linear regression and predict the output.
#Developed by: Azeez Ahamad
#Ref.No: 23003977

import pandas as pd
from sklearn import linear_model
import matplotlib.pyplot as plt

df=pd.read_csv("cars.csv")

x=df[['Weight', 'Volume']]
y=df['CO2']

regr=linear_model.LinearRegression()
regr.fit(x,y)

#coefficients and intercept of model
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2= regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:

### Insert your output

![Screenshot 2023-12-25 170213](https://github.com/Yashvanth21/Multivariate-Linear-Regression/assets/144979957/8d9bd2d9-c102-4a39-b65a-ac4f5e904ea1)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
