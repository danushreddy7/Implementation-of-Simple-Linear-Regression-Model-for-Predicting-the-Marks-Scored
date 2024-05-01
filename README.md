# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the standard Libraries. 
2. .Set variables for assigning dataset values.
3. .Import linear regression from sklearn.
4. Assign the points for representing in the graph. 5.Predict the regression for marks by using the representation of the graph. 6.Compare the graphs and hence we obtained the linear regression for the given datas

## Program:
import pandas as pd
df=pd.read_csv('/content/Untitled spreadsheet - Sheet1.csv')
df
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
df=pd.read_csv('/content/Untitled spreadsheet - Sheet1.csv')
df.head(10)
plt.scatter(df['X'],df['Y'])
plt.xlabel('X')
plt.xlabel('Y')
X=df.iloc[:,0:1]
Y=df.iloc[:,-1]
Y
from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test=train_test_split(X,y,test_size=0.2,random_state=0)
from sklearn.linear_model import LinearRegression
lr=LinearRegression()
lr.fit(X_train,Y_train)
X_train
Y_train
lr.predict(X_test.iloc[0].values.reshape(1,1))
plt.scatter(df['X'],df['Y'])
plt.xlabel('X')
plt.xlabel('Y')
plt.plot(X_train,lr.predict(X_train),color='red')
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: T.DANUSH REDDY
RegisterNumber:212223040029  
*/
```

## Output:
# HEAD:
![image](https://github.com/danushreddy7/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/149035740/1f37a114-0074-48bb-9424-9a0202f0fdd3)
# GRAPH OF PLOTTED DATA:
![image](https://github.com/danushreddy7/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/149035740/cd855cba-abae-45bc-9252-75424b22c347)
# TRAINED DATA:
![image](https://github.com/danushreddy7/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/149035740/d0da20d0-9210-4b52-ad7f-6fe32dfe04df)
# LINE OF REGRESSION:
![image](https://github.com/danushreddy7/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/149035740/45009684-bc33-4f14-963f-eff4b6116e92)
# COEFFICIENT AND INTERCEPT VALUES:
![image](https://github.com/danushreddy7/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/149035740/eabd8908-f670-43b6-af73-eb931700056a)



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
