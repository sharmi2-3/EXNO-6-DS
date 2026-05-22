# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np

df=pd.read_csv('/content/titanic_dataset.csv')
df
```
.
<img width="1468" height="520" alt="image" src="https://github.com/user-attachments/assets/8a650d0f-5b31-4b4f-9bcb-8a4f0282fef0" />
.
```
sns.displot(df['Age'])
plt.title("Distribution of Age")
plt.show()
```
.
<img width="489" height="512" alt="image" src="https://github.com/user-attachments/assets/c8b71b37-c8da-47b3-bda7-57d4f1f5c628" />
```
sns.countplot(x='Pclass', data=df)
plt.title("Passenger class count")
plt.show()
```
.
<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/17652195-fbca-4ec6-8cc3-c2b8034b4266" />
.
```
sns.countplot(df['Sex'])
plt.title("Distribution of sex")
plt.show()
```
.
<img width="601" height="455" alt="image" src="https://github.com/user-attachments/assets/77e46818-6f10-41dc-9f8f-434e0aef0a84" />

```
sns.countplot(x='Sex', hue='Survived', data=df)
plt.title("Survival based on Gender")
plt.show()
```
.
<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/61960541-17ef-49e5-9ee9-9c3991b7dd46" />

```
sns.boxplot(x='Pclass', y='Age', data=df)
plt.title("Age Distribution by Passenger Class")
plt.show()
```
.
<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/360e3db4-6dc9-4ccf-a492-1715918448fc" />

```
numeric_df = df.select_dtypes(include=['number'])

sns.heatmap(numeric_df.corr(), annot=True)
plt.title("Correlation Heatmap")
plt.show()
```
.
<img width="596" height="505" alt="image" src="https://github.com/user-attachments/assets/dc3ae17d-785d-466e-b022-2d6136469537" />


# Result:
Thus, the data visualization techniques using seaborn has been executed successfully. `
