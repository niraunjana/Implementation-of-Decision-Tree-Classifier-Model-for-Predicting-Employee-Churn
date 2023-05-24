# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

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
Developed by  : NIRAUNJANA GAYATHRI G R
RegisterNumber: 22008369

import pandas as pd
data=pd.read_csv("/content/Employee.csv")

print("data.head")
data.head()

print("data.info()")
data.info()

print("isnull() and sum()")
data.isnull().sum()

print("data value counts()")
data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data ["salary"]=le.fit_transform(data["salary"])
print(" data.head() for salary")
data.head()


x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
print("x.head()")
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
print("accuracy value")
accuracy

print("data prediction")
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/4b9430d2-56c8-4ad2-99e1-350903fab7a2)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/2a68c535-6615-47cf-8859-55df1c245293)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/7ac0b760-7ed1-4307-895e-fe8fe69ee08c)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/0499bcc9-a04e-475f-a18d-c136da9ff521)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/4b5b7f0a-13a4-43c6-a238-1f1856f54ad0)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/46ed56c6-e7ec-453e-8785-2836cee65200)

![image](https://github.com/niraunjana/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119395610/834f86c7-3497-42f9-9d6c-c10bdbafa63e)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
