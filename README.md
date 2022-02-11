# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
import pandas as pd.
<br>

### Step2:
Read the csv file.
<br>

### Step3:
Get the value of X and y variables.
<br>

### Step4:
Create the linear regression model and fit.
<br>

### Step5:
predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.
<br>

## Program:
```python
##Developed by : Naramala Niharika
##Reference number: 21500912
import pandas as pd

from sklearn import linear_model

df =pd.read_csv("cars.csv")

x= df[["Weight","Volume"]]

y= df["CO2"]

regr =linear_model.LinearRegression()

regr.fit(x,y)

print("coefficients: ",regr.coef_
)
print("Intercept: ",regr.intercept_)

predictedco2=regr.predict([[3000,1200]])

print("Predicted co2 for the coressponding weight and volume ",predictedco2)

```
## Output:
![Output](https://github.com/naramala-niharika/Multivariate-Linear-Regression/blob/master/u1.PNG?raw=true)

## Result:
Thus the multivariate linear regression is implemented and predicted the output using python program.