# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import the necessary packages using import statement. 2.Read the given csv file and print the number of contents to be displayed. 3.Split the dataset using train_test_split. 4.Calculate Y_Pred and accuracy. 5.Display the result.

Program:

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: PAVAN KISHORE.M
RegisterNumber:  212221230076


import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["EmailText"].values
y=data["Label"].values
from sklearn.model_selection import train_test_split 
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
  
*/
```

## Output:
## data.head()
![t1](https://user-images.githubusercontent.com/94154941/173226759-d9a194e7-a509-4f77-871d-dfb60d5c1bc6.png)
## data.info()
![t2](https://user-images.githubusercontent.com/94154941/173226765-19b7eda0-d6b4-47e5-8aae-deddcb763d78.png)
## Data.isnull().sum()
![t3](https://user-images.githubusercontent.com/94154941/173226780-7e8196a6-ce59-447c-a0bd-decb8db168ac.png)
## y_pred
![t4](https://user-images.githubusercontent.com/94154941/173226787-423cacb0-893d-41c2-8cfd-d4d24c167da4.png)
## accuracy
![t5](https://user-images.githubusercontent.com/94154941/173226802-7588c982-8065-4ad1-b551-1513667b76b2.png)



## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
