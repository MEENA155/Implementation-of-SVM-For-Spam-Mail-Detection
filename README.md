# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

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
Developed by: MEENA .S
RegisterNumber:212221240028
import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extractiaon.text import CountVectorizer
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
## Data Head:
![image](https://user-images.githubusercontent.com/94677128/174335267-42f5470c-a4dc-4306-ae91-69723203b94f.png)
## Data Info:
![image](https://user-images.githubusercontent.com/94677128/174335368-d3fb70e0-e8e8-48e2-8043-a2353d1a0775.png)
## Data isnull():
![image](https://user-images.githubusercontent.com/94677128/174335435-c493a2c7-0d51-49d9-b192-3bdbcec7e3bb.png)
## y_pred:
![image](https://user-images.githubusercontent.com/94677128/174335508-7bf27ced-47d2-4d22-a9a6-e49080ddfe0c.png)
## Accuracy:
![image](https://user-images.githubusercontent.com/94677128/174335558-35953be3-d7fa-4a2a-b8bf-75b889eb3ede.png)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
