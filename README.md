# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import required libraries. 
2.Load dataset using pandas.read_csv(). 
3.Separate Level (X) and Salary (y). 
4.Train the DecisionTreeRegressor model. 
5.Predict salary for the given level and display the result.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:RAJAPRABU.S 
RegisterNumber:212225240113  
*/
import pandas as pd from sklearn.tree import DecisionTreeRegressor import matplotlib.pyplot as plt

data = pd.read_csv("C:/Users/acer/Downloads/Salary.csv")

X = data[['Level']] y = data['Salary']

model = DecisionTreeRegressor()

model.fit(X, y)

level = float(input("Enter the employee level: ")) predicted_salary = model.predict([[level]])

print("Predicted Salary:", predicted_salary[0])

plt.scatter(X, y, color='red') plt.plot(X, model.predict(X), color='blue') plt.xlabel("Level") plt.ylabel("Salary") plt.title("Decision Tree Regression") plt.show()
```

## Output:
<img width="716" height="607" alt="image" src="https://github.com/user-attachments/assets/c4371c18-2e9b-46ea-ba12-7d742a38a1c8" />

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
