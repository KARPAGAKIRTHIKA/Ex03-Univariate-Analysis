# Ex03-Univariate-Analysis

## Aim
To read the given data and perform the univariate analysis with different types of plots.

## Explanation
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm

Step1
Read the given data.

Step2
Get the information about the data.

Step3
Remove the null values from the data.

Step4
Mention the datatypes from the data.

Step5
Count the values from the data.

Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program

import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()

df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)

## Output

## DATA

![image](https://user-images.githubusercontent.com/103020162/228204354-41cfba5a-7e96-4758-870a-eda97846e05d.png)


## DATA HEAD

![image](https://user-images.githubusercontent.com/103020162/228204822-9891e991-561c-46ea-8523-d5ac6e3871c1.png)


## DATA INFORMATION

![image](https://user-images.githubusercontent.com/103020162/228205123-7ceac31a-cbbf-4e38-b66b-2dd6d8645dfc.png)


## DATA DESCRIBE

![image](https://user-images.githubusercontent.com/103020162/228205293-9e9f690c-b8e8-42dd-b5f7-62858498979c.png)


## DATA NULL VALUES

![image](https://user-images.githubusercontent.com/103020162/228205557-316c11c8-e71c-451f-837d-06f31a1d6672.png)


## DATA'S DATATYPES

![image](https://user-images.githubusercontent.com/103020162/228205711-68df1998-3549-40be-ba1b-525b66aed5e2.png)


## DATA'S VALUECOUNT

![image](https://user-images.githubusercontent.com/103020162/228205976-f512149e-2d46-4a11-b10d-91392050e45c.png)


## BOXPLOT

![image](https://user-images.githubusercontent.com/103020162/228206157-21892f15-87a4-4edf-98c2-b7748d7986fb.png)


## COUNTPLOT

![image](https://user-images.githubusercontent.com/103020162/228206241-52097c6d-4ebf-4975-beff-1fbaa1a45310.png)


## DISTRIBUTION PLOT

![image](https://user-images.githubusercontent.com/103020162/228206431-29821660-58bc-468b-8e34-28a3084952d7.png)


## HISTOGRAM PLOT

![image](https://user-images.githubusercontent.com/103020162/228206567-9ff80dca-e9cf-41dd-bad0-9ffac89e7667.png)

## Result

Thus we have read the given data and performed the univariate analysis with different types of plots.
