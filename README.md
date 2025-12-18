# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1

import pandas as pd.


### Step2

Read the csv file.


### Step3

Get the value of X and y variables


### Step4

Create the linear regression model and fit.


### Step5

Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```

Developed by : SANTHOSHKUMAR . J
Reg No : 25016468
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)




```
## Output:
<img width="916" height="96" alt="Screenshot 2025-12-18 111546" src="https://github.com/user-attachments/assets/6ec43e8c-9988-40ee-914f-60af6ff9236d" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
