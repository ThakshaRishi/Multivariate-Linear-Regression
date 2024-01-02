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
Read the CSV file using pd.read_csv()

### Step3
Get the values from the user as input

### Step4
Create a linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3 and print the output.

## Program:
```
#Developed by: Thaksha Rishi
#Register Number: 212223100058
import pandas as pd
from sklearn import linear_model as lm
df=pd.read_csv('rishi.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=lm.LinearRegression()
regr.fit(a,b)
print("Coefficient ",regr.coef_)
print("Intercept ",regr.intercept_)
print("Amount ",regr.predict([[3300,1300]]))





```
## Output:
![Screenshot 2024-01-02 224435](https://github.com/ThakshaRishi/Multivariate-Linear-Regression/assets/144870423/77a4bf4f-2917-4390-b7b5-803ee93c509e)
![Screenshot 2024-01-02 224446](https://github.com/ThakshaRishi/Multivariate-Linear-Regression/assets/144870423/7768129b-9582-4252-86d9-9bf90f4bcc30)


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
