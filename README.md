# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>import pandas library

### Step2
<br>Import Linear_model from sklearn.


### Step3
<br>Read the csv file using pandas library.


### Step4
<br> Enter the parameters of the linear function.

### Step5
<br> print the parameters of the linear function.


## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
x = df[['Weight', 'Volume']]
y= df['c02']
regr = linear_model.LinearRegression()
regr.fit(x, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedc02 = regr.predict(pd.DataFrame([[3300,1300]], columns=['Weight', 'Volume']))
print('Predicted C02 for the corresponding weight and volume:', predictedc02)





```
## Output:
<img width="877" height="152" alt="image" src="https://github.com/user-attachments/assets/cf2543c4-bfa8-49bb-bb05-50afb871219a" />


### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
