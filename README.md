# Ex-03 UNIVARIATE ANALYSIS
## AIM
To read the given data and perform the univariate analysis with different types of plots.

## EXPLANATION
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## ALGORITHM
Step1:Read the given data.

Step2:Get the information about the data.

Step3:Remove the null values from the data.

Step4:Mention the datatypes from the data.

Step5:Count the values from the data.

## PROGRAM:
```
Developed By : PRADEEPASRI S
Register Number : 212221220038
```
## superstore.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv('/content/SuperStore (1).csv')
print(df)
df.head()
df.info()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
df.describe()
```
## employeesal.csv
```
import pandas as pd
df=pd.read_csv("/content/employeesal (1).csv")
df
df.info()
df.dtypes
df['Salary'].value_counts()
df.describe()
import seaborn as sns
sns.boxplot(x='Experience_Years',data=df)
sns.countplot(x="Experience_Years",data=df)
sns.distplot(df['Experience_Years'])
sns.histplot(x="Experience_Years",data=df)
df.skew()
sns.histplot(x='Salary',data=df)
sns.distplot(df['ID'])
df.kurtosis()
sns.boxplot(x='Salary',data=df)
sns.boxplot(x='Experience_Years',data=df)
```
## diabetes.csv
```
import pandas as pd
import numpy as np
import seaborn as sns
df = pd.read_csv("/diabetes.csv")
df
df.info()
df.isnull().sum()
df.dtypes
df.describe()
df['Glucose'].value_counts()
sns.boxplot(x="Glucose",data=df)
sns.countplot(x="Glucose",data=df)
sns.distplot(df['Glucose'])
sns.histplot(x="Glucose",data=df)
df.skew()
df.kurtosis()
```
## OUTPUT
## superstore.csv
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/8f826cab-767b-43d7-926a-8440a65fe2c2)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/2b712a50-e488-4d0b-bae8-ac9ce5090a4b)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/c1cbcd16-3856-42f8-a51e-54c05237d035)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/aa4f1a34-22d8-4bf9-89e8-b46fb4f86479)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/d4b3cd54-d08e-4813-9ecb-04a26b8d0775)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/4cc67202-5ebd-4fdc-982e-784037cc0f76)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/5e98d7cb-b509-45ac-a127-3c98a6a08f38)
## employeesal.csv
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/cae00b4b-bf96-401d-b304-5c833114f53e)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/112ec929-6f6f-47cf-8713-a1a78a7155fd)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/4b66efee-a4b0-46c7-987b-fa3b00a3a15b)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/e28a6849-48a2-42f0-bf47-da3836b0a806)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/e797ff77-df6a-4991-a0a8-a11579e15383)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/87366552-07ce-430a-ba46-33f0108ceb54)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/cca678dd-70cb-4b66-b07b-4b08ddc38354)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/4cfa87ef-b93c-4513-9ebe-b64610ef04bb)
## diabetes.csv
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/769ae994-c04f-48ae-8d7d-8cee3b146ec7)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/b6494943-496b-49ae-902a-78d5881fe59d)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/a1bf94f0-5b35-4bb3-9645-e31ccb4cae1a)
![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/23a157c4-522b-4635-804a-bb5b0b6a9e05)

![image](https://github.com/pradeepasri26/ODD2023-DataScience-Ex-03/assets/131433142/eb4e7c1c-ddd4-4a48-aff8-bd9191484881)

## RESULT
Hence the univariate analysis is verified.


















