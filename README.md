# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.  Import the necessary packages using import statement.
2.  Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().
3.  Import KMeans and use for loop to cluster the data.
4.  Predict the cluster and plot data graphs.
5.  Print the outputs and end the program 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: PRAISEY S 
RegisterNumber: 212222040117
import pandas as pd
import numpy as np
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
l=LabelEncoder()
data["salary"]=l.fit_transform(data["salary"])
data.head()
data["Departments "]=l.fit_transform(data["Departments "])
data.head()
data.info()
data.shape
x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','Departments ','salary']]
x.head()
x.shape
x.info()
y=data['left']
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
print("Accuracy = ",accuracy)
dt.predict([[0.5,0.8,9,260,6,0,1,2,1]]) 
*/
```

## Output:

Read csv file:

![out 6 1](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/a4b55eba-0a81-4fdb-a391-4258c481a101)

Dataset info:

![out 6 2](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/869cdfb6-1f73-4d79-9ade-0b374051acdf)

![out 6 22](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/f7c1f5d7-95f0-4a50-b32c-74d02079e277)

Dataset Value count:

![out 6 3](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/85c667bc-666c-4fec-93db-f0ac02d78e45)

Dataset head:

![out 6 4](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/790dcec7-a12b-47f1-897f-54562cbafc8a)

Data info:

![out 6 5](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/9be93393-a8d4-4c9b-b15e-32fc67522279)

Dataset shape:

![out 6 61](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/a4a32913-a721-46c1-8359-6d0f162bd6fe)

![out 6 6](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/e5a73365-d275-483d-86a7-15d1a692e4bb)

Y-Pred:

![out 6 7](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/c1d5e5aa-6bfe-4698-9f43-57899eb4e575)

Accuracy:

![out 6 8](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/b8317954-1b40-4705-b4cd-20ffc26e08a4)

Dataset Predict:

![out 6 9](https://github.com/PRAISEYSOLOMON/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119394259/2295c09a-d43d-48d8-b04e-030b533ced1b)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
