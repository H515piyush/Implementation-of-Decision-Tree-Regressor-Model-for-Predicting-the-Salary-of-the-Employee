# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:Piyush kumar 
RegisterNumber:212223220075  
*/

import pandas as pd
 data=pd.read_csv("C:/Users/admin/OneDrive/Desktop/Salary.csv")
 data.head()
 data.info()
 data.isnull().sum()
 from sklearn.preprocessing import LabelEncoder
 le=LabelEncoder()
 data['Position']=le.fit_transform(data['Position'])
 data.head()
 x=data[['Position','Level']]
 y=data['Salary']
 from sklearn.model_selection import train_test_split
 x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_stat
 from sklearn.tree import DecisionTreeClassifier
 dt=DecisionTreeClassifier()
 dt.fit(x_train,y_train)
 y_predict=dt.predict(x_test)
 from sklearn import metrics
 mse=metrics.mean_squared_error(y_test,y_predict)
 mse
 r2=metrics.r2_score(y_test,y_predict)
 r2
dt.predict([[5,6]])
 
 
```



## Output:

![Screenshot 2024-04-02 103329](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/2d697051-83ab-4293-b890-e8bd31011078)

![Screenshot 2024-04-02 102109](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/205e08b8-78d0-4bb2-aed4-f0ed7c3ea3cb)

![Screenshot 2024-04-02 102117](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/8071453a-0db4-449e-aaba-3a15e940c084)

![Screenshot 2024-04-02 102124](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/bb3d6dcf-4a92-413c-b0a5-156ac5f61519)

![Screenshot 2024-04-02 102140](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/a0815aec-b92f-4352-b8d0-bb31fe107d1c)
![Screenshot 2024-04-02 102146](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/572ecaa2-7018-4c22-a63d-86ec4e627d7a)

![Screenshot 2024-04-02 102151](https://github.com/H515piyush/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/147472999/139ccb0b-6960-4ca5-a781-21cbe2d51d7f)




## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
