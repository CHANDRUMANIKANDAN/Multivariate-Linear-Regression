# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
import pandas as pd.

Step2
Read the CSV file.

Step3
Get the value of x and y variables.

Step4
Create the linear regression model and fit.

Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

Step6
Print the predicted output.
## Program:
```

##Developed by:CHANDRU M
##REGISTER NUMBER: 22009010

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")

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
![output3](https://user-images.githubusercontent.com/118644502/214355464-0d6c5585-42e4-4f67-a2fe-068d6e1dc03b.jpg)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
