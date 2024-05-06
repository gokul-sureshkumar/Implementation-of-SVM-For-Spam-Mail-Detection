# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program
2. Import the python pandas library as pd
3. Read the contents of the Spam csv file
4. Display the first 5 rows of the dataset using head()
5. Assign x as v1 values and y as v2 values
6. From sklearn library select the feature extraction and import CountVectorizer
7. CountVectorizer will convert the Text to Numerical Data
8. From sklearn library import Support Vector Classifier (ie. SVC)
9. Predict the x_test using SVC
10. Print the accuracy of the SVM Model 11.Stop the program
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: AGOKUL S
RegisterNumber: 212222110011
*/
```
```
/*
import chardet
file='/content/spam.csv'
with open(file, 'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding = 'Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()

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

## 1. Result output
![ml 9 i1](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/3eab037b-6809-422e-873d-f9ed78e8a1ad)
## 2. data.head()
![ml 9 i2](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/bef21527-e9ef-4e71-bfa4-15658495faa7)
## 3. data.info()
![ml 9 i3](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/ea4dfc15-dd68-4050-b0d9-c601412d8074)
## 4. data.isnull().sum()
![ml 9 i4](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/ccbf5240-2004-4419-a299-71feccb702bb)
## 5. Y_prediction value
![ml 9 i5](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/c4cb968d-d084-4389-9350-d6632f19b874)
## 6. Accuracy value
![ml 9 i6](https://github.com/Rama-Lekshmi/Implementation-of-SVM-For-Spam-Mail-Detection/assets/118541549/e8577b82-305d-43be-ac7b-5e830b680157)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
