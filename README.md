<H3>ENTER YOUR NAME : LAVANYA S</H3>
<H3>ENTER YOUR REGISTER NO : 212223230112 </H3>
<H3>EX. NO.1</H3>
<H3>DATE : 29-04-2026</H3>
<H1 ALIGN =CENTER> Introduction to Kaggle and Data preprocessing</H1>

## AIM:

To perform Data preprocessing in a data set downloaded from Kaggle

## EQUIPMENTS REQUIRED:
Hardware – PCs
Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## RELATED THEORETICAL CONCEPT:

**Kaggle :**
Kaggle, a subsidiary of Google LLC, is an online community of data scientists and machine learning practitioners. Kaggle allows users to find and publish data sets, explore and build models in a web-based data-science environment, work with other data scientists and machine learning engineers, and enter competitions to solve data science challenges.

**Data Preprocessing:**

Pre-processing refers to the transformations applied to our data before feeding it to the algorithm. Data Preprocessing is a technique that is used to convert the raw data into a clean data set. In other words, whenever the data is gathered from different sources it is collected in raw format which is not feasible for the analysis.
Data Preprocessing is the process of making data suitable for use while training a machine learning model. The dataset initially provided for training might not be in a ready-to-use state, for e.g. it might not be formatted properly, or may contain missing or null values.Solving all these problems using various methods is called Data Preprocessing, using a properly processed dataset while training will not only make life easier for you but also increase the efficiency and accuracy of your model.

**Need of Data Preprocessing :**

For achieving better results from the applied model in Machine Learning projects the format of the data has to be in a proper manner. Some specified Machine Learning model needs information in a specified format, for example, Random Forest algorithm does not support null values, therefore to execute random forest algorithm null values have to be managed from the original raw data set.
Another aspect is that the data set should be formatted in such a way that more than one Machine Learning and Deep Learning algorithm are executed in one data set, and best out of them is chosen.


## ALGORITHM:
STEP 1:Importing the libraries<BR>
STEP 2:Importing the dataset<BR>
STEP 3:Taking care of missing data<BR>
STEP 4:Encoding categorical data<BR>
STEP 5:Normalizing the data<BR>
STEP 6:Splitting the data into test and train<BR>

##  PROGRAM:
```
from google.colab import files
import pandas as pd
import io
from sklearn.preprocessing import StandardScaler
from sklearn.preprocessing import MinMaxScaler
from sklearn.model_selection import train_test_split
df.isnull().sum()
df.fillna(0)
df.duplicated()
df['EstimatedSalary'].describe()
scaler = StandardScaler()
inc_cols = ['CreditScore', 'Tenure', 'Balance', 'EstimatedSalary']
scaled_values = scaler.fit_transform(df[inc_cols])
df[inc_cols] = pd.DataFrame(scaled_values, columns = inc_cols, index = df.index)
df
x = df.iloc[:, :-1]
y = df.iloc[:, -1]
print("X Values")
x
print("Y Values")
y
x_train, x_test, y_train, y_test = train_test_split(x, y, test_size = 0.2, random_state = 42)
print("X Training data")
x_train
print("X Testing data")
x_test
print(len(x_test))
print(len(y_test))

```


## OUTPUT:
<img width="1432" height="716" alt="image" src="https://github.com/user-attachments/assets/b07755d8-fefe-40af-b729-6df302a5bd4c" />

<img width="1100" height="602" alt="image" src="https://github.com/user-attachments/assets/bf5c6790-9065-4f73-98d4-1bd6b6d948b4" />

<img width="1366" height="506" alt="image" src="https://github.com/user-attachments/assets/8ff6cd26-b64d-4301-aa97-9302c0025dde" />

<img width="975" height="792" alt="image" src="https://github.com/user-attachments/assets/78afeb26-9e2a-4b61-a65f-818a6262008c" />

<img width="1428" height="609" alt="image" src="https://github.com/user-attachments/assets/8b7c6c1e-9595-4b49-8e10-57f49d9f8516" />

<img width="867" height="707" alt="image" src="https://github.com/user-attachments/assets/34cfaa14-12e8-4bf8-a19a-fff405bcc9e7" />

<img width="1399" height="606" alt="image" src="https://github.com/user-attachments/assets/1963d6da-3106-4984-a6eb-f2d589741906" />

<img width="1399" height="606" alt="image" src="https://github.com/user-attachments/assets/a7200bf7-5546-
4f63-afb3-3aac9cbe6353" />

<img width="1375" height="737" alt="image" src="https://github.com/user-attachments/assets/c9af918b-04e5-4100-894c-3a378b84c866" />


## RESULT:
Thus, Implementation of Data Preprocessing is done in python  using a data set downloaded from Kaggle.


