# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Start the program

2.Import the required Python libraries

3.Create the dataset containing hours studied and marks scored

4.Separate the independent variable (hours studied) and dependent variable (marks scored)

5.Create a Simple Linear Regression model

6.Train the model using the given dataset

7.Use the trained model to predict the marks scored

Display the slope and intercept of the regression line

Plot the actual data points and the regression line

Stop the program


## Program:
```
# Import required libraries
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

# Load the dataset
data = pd.read_csv("data.csv")

# Independent variable (X) and Dependent variable (y)
X = data[['Experience']]   # must be 2D
y = data['Salary']

# Create the Linear Regression model
model = LinearRegression()

# Train the model
model.fit(X, y)

# Predict values
y_pred = model.predict(X)

# Display slope and intercept
print("Slope (m):", model.coef_[0])
print("Intercept (c):", model.intercept_)

# Plot the data and regression line
plt.scatter(X, y)
plt.plot(X, y_pred)
plt.xlabel("Experience")
plt.ylabel("Salary")
plt.title("Simple Linear Regression")
plt.show()
```
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Sunil kumar R
RegisterNumber: 212225040440


## Output:
![screenshot](https://github.com/user-attachments/assets/e8e64d25-dcc2-48f4-a485-c5e17a1b84be)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
