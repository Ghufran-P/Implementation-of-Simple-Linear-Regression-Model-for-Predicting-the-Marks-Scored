# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Input dataset X (hours studied) and Y (marks), and reshape X.
2.Import and initialize the Linear Regression model.
3.Train the model using the given data (fit).
4.Extract slope m and intercept b.
5.Take user input and predict marks using the model.
6.Plot actual data and regression line for visualization. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: MOHAMMED GHUFRAN P
RegisterNumber:  212225230178
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression


X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])

model = LinearRegression()

model.fit(X, Y)

m = model.coef_[0]
b = model.intercept_

print("Slope (m):", m)
print("Intercept (b):", b)

x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])

Y_pred = model.predict(X)

plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression (Using sklearn)")
plt.legend()
plt.show()
*/
```

## Output:
<img width="929" height="685" alt="image" src="https://github.com/user-attachments/assets/a8ab3bed-c82d-46b8-ad89-9f465acfabeb" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
