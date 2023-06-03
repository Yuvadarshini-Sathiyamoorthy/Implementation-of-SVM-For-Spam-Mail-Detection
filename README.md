# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required packages.
2. Import the dataset to operate on.
3. Split the dataset.
4. Predict the required output.
5. End the program.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: Yuvadarshini S
RegisterNumber: 212221230126 

import pandas as pd
data=pd.read_csv("spam.csv",encoding='Windows-1252')

import chardet
file='spam.csv'
with open(file, 'rb') as rawdata:
    result = chardet.detect(rawdata.read(10000))
result

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

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
## Result output
![91](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/8c2a20bf-1ff1-46fc-adfa-a92e9e686e9e)

## data.head()
![92](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/4868350d-bba7-40e3-84ab-a5fac70ef1d9)

## data.info()
![93](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/cc1fe2a7-11d0-49e4-9a92-b2d520c8ebe3)

## data.isnull().sum()
![94](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/581f80ef-e39a-4445-b3d3-03aba26fbdae)

## Y_prediction value
![95](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/40a0a3b6-b0b2-4a90-8ddb-ec7683f387c6)

## Accuracy value
![96](https://github.com/Yuvadarshini-Sathiyamoorthy/Implementation-of-SVM-For-Spam-Mail-Detection/assets/93482485/dce8e7c5-8b01-4ee6-b16d-baf124139b70)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
