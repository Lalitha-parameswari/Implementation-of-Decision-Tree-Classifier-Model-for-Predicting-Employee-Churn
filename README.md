# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import pandas library to read csv or excel file.
2. Import LabelEncoder using sklearn.preprocessing library.
3. Transform the data's using LabelEncoder.
4. Import decision tree classifier from sklearn.tree library to predict the values.
5. Find accuracy.
6. Predict the values.
7. End of the program.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: LALITHA PARAMESWARI.C
RegisterNumber: 212219220027
import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics 
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:

## HEAD:

![image](https://user-images.githubusercontent.com/103946827/174734730-5dded206-90a2-4c20-9afd-94b48c1d042a.png)

## INFO:

![image](https://user-images.githubusercontent.com/103946827/174734820-910adc15-be30-48b3-9126-c99d6cdc2735.png)

## ISNULL:

![image](https://user-images.githubusercontent.com/103946827/174735019-7efc3afa-c891-4096-becd-a4e094f44004.png)

## LEFT:

![image](https://user-images.githubusercontent.com/103946827/174735098-00542979-db39-4218-ba9b-92b80ff0c504.png)

## HEAD USING LABELENCODER:

![image](https://user-images.githubusercontent.com/103946827/174735173-b1424a20-b59e-4f43-aeb3-f8cf0deb3396.png)

## ACCURACY:

![image](https://user-images.githubusercontent.com/103946827/174735300-48c58c4f-e954-4344-9508-ed4a0fff00f6.png)

## PREDICT:

![image](https://user-images.githubusercontent.com/103946827/174735351-f0868564-844b-4ccc-b24b-6fa4778cb337.png)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
