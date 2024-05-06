# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:


> Developed By: SANJAY T

> REG NO: 212222110039
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/7c65f491-5956-4e9c-a160-9fbced92429b)
![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/e69fbee6-5d4c-489a-8112-1182b02b69c7)




### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/c0a225cd-f456-4589-a822-78e495614e8a)

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/c63ca57c-9548-4506-afd0-ef90d0f602ff)



### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```


![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/5e130a18-d7d1-4220-8333-b8a10883c3d7)

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/bd05f0e4-ebf4-461f-b6f6-8e2255d0f976)




### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/d99b5488-997f-49ca-bb88-415af125095c)




### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/331aa11c-faa6-4097-81c2-41e898ba371f)



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/8f7b3b5f-b5ec-47a9-b5e7-d342039e3840)




### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/5a6587c5-bb09-4fbb-b1b5-5caba40a5ab7)



```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![image](https://github.com/sanjaythiyagarajan/EXNO-5-DS/assets/119409242/e2704276-9052-431f-804c-c8d20022aedc)



## Result:

### Thus, all the data visualization techniques of matplotlib has been implemented.
