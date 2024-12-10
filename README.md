# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the pandas library as pd.
### Step2
Read the csv file.
### Step3
Get the values of x and y as inputs.
### Step4
Create the linear regression model and fit.
### Step5
Predict the CO2 emission of a car using the given specifications.
## Program:

```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car (1).csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)
```
## Output:

![Screenshot 2024-12-10 181005](https://github.com/user-attachments/assets/87e81c56-e7be-415e-bcbf-ac7df3f69228)


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
