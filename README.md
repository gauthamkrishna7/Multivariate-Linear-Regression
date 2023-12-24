# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.

### Step2
Import Linear_model from sklearn.

### Step3
Read the csv file using pandas library.

### Step4
Enter the parameters of the linear function.

### Step5
Print the parameters of the linear function.

## Program:
```Python
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
<img width="695" alt="image" src="https://github.com/Nijeesh-bit/Multivariate-Linear-Regression/assets/89188014/64a18346-192e-44d7-8828-c0b38da95da9">
<img width="921" alt="image" src="https://github.com/Nijeesh-bit/Multivariate-Linear-Regression/assets/89188014/0029765b-35be-4917-b83e-80c99b881ced">

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
