# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Select any online compiler.
### Step2
Type the required coding.
### Step3
Import pandas.
### Step4
Take a screenshot of the output and copy the program and the output in your git repository.
### Step5
Push the output images and program in the git repository.

## Program:
```
'''
Developed by: HARI PRASATH S
Reference number: 212222240034
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![283502074-df5b302d-fa12-4050-9e4c-1414d1b44caf](https://github.com/hariprasath5106/Multivariate-Linear-Regression/assets/111515488/d58b8da3-9823-4497-9b74-98f47c86d4ee)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
