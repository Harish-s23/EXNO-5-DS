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
```
NAME: HARESH R
REG NO: 212224040097
```
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['Billie','Travis','Kendric','Weeknd']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
```

<img width="751" height="538" alt="Screenshot 2025-10-27 104437" src="https://github.com/user-attachments/assets/f8a2d8f5-7076-49f1-b1dd-2a3e9bae8ea7" />

```
student=['Billie','Travis','Kendric','Weeknd']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```
<img width="748" height="538" alt="Screenshot 2025-10-27 104453" src="https://github.com/user-attachments/assets/07fdf38a-aaa8-4692-92a6-09347da6cee7" />


### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
```
<img width="691" height="514" alt="Screenshot 2025-10-27 104551" src="https://github.com/user-attachments/assets/95dd46d8-f6e2-4e76-ae55-7d2679267136" />

```
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

<img width="702" height="569" alt="Screenshot 2025-10-27 104609" src="https://github.com/user-attachments/assets/a94ffac8-66a3-486c-afc8-e2836102a8ba" />


### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="561" height="520" alt="Screenshot 2025-10-27 104654" src="https://github.com/user-attachments/assets/ebd660f4-e30a-47cf-8cf1-24f3f1f8ee06" />

```
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="553" height="497" alt="Screenshot 2025-10-27 104707" src="https://github.com/user-attachments/assets/69fc3ffd-fc89-4666-9842-d6e5f140da1b" />



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
<img width="693" height="512" alt="Screenshot 2025-10-27 104823" src="https://github.com/user-attachments/assets/1ed21ea3-76df-4057-8ca0-43d704734b03" />


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
<img width="701" height="568" alt="Screenshot 2025-10-27 104911" src="https://github.com/user-attachments/assets/20b07b88-f2b4-47af-b86d-83480260dc7e" />



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='black', alpha=0.5)
plt.show()
```

<img width="666" height="512" alt="Screenshot 2025-10-27 104942" src="https://github.com/user-attachments/assets/564e9a5f-3f5d-46c7-85ea-472e6477bee0" />




### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="1274" height="455" alt="Screenshot 2025-10-27 105048" src="https://github.com/user-attachments/assets/05b6d90d-1266-44d9-b50c-80256dd25798" />



```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="724" height="599" alt="Screenshot 2025-10-27 105058" src="https://github.com/user-attachments/assets/67b9da8e-2441-45ff-b031-a674e14355e8" />



## Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
