# workshop-Multivariate-analysis

## AIM:
To perform multivarient analysis on the given data set.

## ALGORITHM:
### STEP1
1.Clean the data

### STEP2
2.Remove outliers

### STEP3
3.Apply the skew function and Kurtosis

### STEP4
4.Apply Bivariate analysis on numerical and categorical

### STEP5
5 .Apply Multivariate analysis

## PROGRAM:

### BIVARIATE ANALYSIS:
```
import pandas as pd
import seaborn as sns
df = pd.read_excel("/content/FlightInformation.xlsx")
df
df.info()
df.describe()
df.isnull().sum()
df.kurtosis()
df.skew()
sns.scatterplot(x=df['Price'],y=df['Duration'],data=df)
sns.boxplot(x=df['Price'],y=df['Duration'])
sns.barplot(x=df['Price'],y=df['Source'],data=df)
sns.set_style('whitegrid')
sns.displot(df,x="Source",hue="Airline")
```
### MULTIVARIATE ANALYSIS:
```
import seaborn as sns
import pandas as pd
import numpy as np
import matplotlib.pyplot as pit
data= pd.read_excel("/content/FlightInformation.xlsx")
data = np.random.randint(low = 1, high = 100, size = (10, 10))
print("The data to be plotted:\n")
print(data)
hm = sns.heatmap(data = data)
pit.show()
df.corr()
```
## OUTPUT:
### DATASET:
![Screenshot 2023-04-10 102733](https://user-images.githubusercontent.com/120232371/230829192-7c0e4bac-7ca1-4487-b719-eff5bf991c77.png)
### INFO:
![Screenshot 2023-04-10 102923](https://user-images.githubusercontent.com/120232371/230829277-13833f8b-a175-4a72-bd5b-1e9fb30aa268.png)
### REMOVING NULL DATA:
![Screenshot 2023-04-10 102923](https://user-images.githubusercontent.com/120232371/230829615-cbba241a-1a07-4562-9e4f-846278e68541.png)
### DESCRIBE:
![Screenshot 2023-04-10 103310](https://user-images.githubusercontent.com/120232371/230829700-2335a1f4-8b49-4134-8a3b-d7384aa4b233.png)
### KURTOSIS:
![Screenshot 2023-04-10 103405](https://user-images.githubusercontent.com/120232371/230829805-700f9910-2307-4a0e-899d-0cc110769c8f.png)
### SKEW:
![Screenshot 2023-04-10 103458](https://user-images.githubusercontent.com/120232371/230829962-befdd6c1-91a3-4f3e-8047-c78b7e3d8862.png)
### SCATTERPLOT:
![Screenshot 2023-04-10 103623](https://user-images.githubusercontent.com/120232371/230830126-67d5843f-1bb7-4834-9429-07044e992143.png)
### BOXPLOT:
![Screenshot 2023-04-10 103712](https://user-images.githubusercontent.com/120232371/230830236-ea9e17aa-9b86-4d7f-ada5-0a0b0c8b2cd5.png)
### BARPLOT:
![Screenshot 2023-04-10 103755](https://user-images.githubusercontent.com/120232371/230830337-f3e217b4-65af-4e44-8994-15a1ec9d00c7.png)
### DISTPLOT:
![Screenshot 2023-04-10 103951](https://user-images.githubusercontent.com/120232371/230830567-a8df30f1-2989-46a0-9e61-e0fd50bf651d.png)
## MULTIVARIATE:

### CORRELATION:
![Screenshot 2023-04-10 104225](https://user-images.githubusercontent.com/120232371/230830828-0c6b16b1-1e66-432b-a413-d14301cc323a.png)
### HEATMAP:
![Screenshot 2023-04-10 104407](https://user-images.githubusercontent.com/120232371/230831002-182c3e8a-a94b-4a53-bb11-b5d5106981cc.png)

## RESULT:
Thus we applied Bivariate/Multivariate Analysis Successfully.




