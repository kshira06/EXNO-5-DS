# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

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
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
```
```
x = [2018, 2019, 2020, 2021, 2022]
y = [15000, 20000, 25000, 30000, 35000]

plt.plot(x, y, 'g*', linestyle='dashed', linewidth=2, markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D Diagram')
plt.show()
```

<img width="909" height="858" alt="image" src="https://github.com/user-attachments/assets/d7837c73-4770-4485-a7e3-44ce881089fa" />

```
plt.subplot(2,2,1)
plt.plot(x,y,'--')
plt.subplot(2,2,2)
plt.plot(x,y,'o--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
plt.show()
```
<img width="816" height="743" alt="image" src="https://github.com/user-attachments/assets/295cc0f2-3732-4049-b1b8-d5f43cb59d6c" />

```
x = np.arange(0, 4*np.pi, 0.1)
y = np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```
<img width="742" height="690" alt="image" src="https://github.com/user-attachments/assets/28cf7856-c6be-49df-b206-9580e5f19fd5" />

```
x = [2, 8, 10]
y = [11, 16, 9]
x1 = [3, 4, 11] 
y1 = [6, 15, 7]
plt.bar(x, y, color='r')
plt.bar(x1, y1, color='g')
plt.title("Bar graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="733" height="816" alt="image" src="https://github.com/user-attachments/assets/e856337d-0e1e-4e60-bc20-1668a6d93925" />

```
x = [1, 2, 3]
y = [7, 3, 9]

plt.plot(x, y, color='g')
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="777" height="770" alt="image" src="https://github.com/user-attachments/assets/ee12a9a9-eb98-4d2b-8b50-2ec61c970717" />

```
x1 = [1, 2, 3]
y1 = [2, 4, 1]
plt.plot(x1, y1, label='line1')

x2 = [1, 2, 3]  
y2 = [4, 1, 3]
plt.plot(x2, y2, label='line2')

plt.title("multiline graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="700" height="796" alt="image" src="https://github.com/user-attachments/assets/ae001699-62f9-464b-ba39-009e71c189b5" />

```
x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth=3, 
         marker='o', markerfacecolor='red', markersize=12, label='spices')
plt.xlim(1, 8)
plt.ylim(1, 8) 
plt.title("line graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="754" height="760" alt="image" src="https://github.com/user-attachments/assets/a1d704b8-307a-4fe0-b9d1-38b71cd01d8b" />

```
yield_apples=[0.895,0.91,0.919,0.926,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='g')
plt.show()
```
<img width="853" height="557" alt="image" src="https://github.com/user-attachments/assets/f069a570-8ff2-4af1-8f0f-031f17a21500" />

```
oranges = [2, 4, 6, 7, 8, 12, 45]
apples = [2, 4, 5, 6, 8, 23, 37]
years = [2019, 2020, 2021, 2022, 2023, 2024, 2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title('Crop yields in Kanto')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.legend(['apples', 'oranges'])  
plt.show()
```
<img width="743" height="732" alt="image" src="https://github.com/user-attachments/assets/f9c75371-e238-4c25-bf59-b2137000671d" />

```
oranges = [2, 4, 6, 7, 8, 12]
apples = [2, 4, 5, 6, 8, 23]
years = [2019, 2020, 2021, 2022, 2023, 2024]
plt.bar(oranges,apples)
plt.plot(years, apples, label='apples', marker='*')
plt.plot(years, oranges, label='oranges', marker='o')
plt.title('Fruit sales')  
plt.xlabel('Year')  
plt.ylabel('Sales')  
plt.legend()  
plt.show()
```
<img width="766" height="743" alt="image" src="https://github.com/user-attachments/assets/e9886d1f-5ec0-4610-bf67-5cea7ec49c29" />

```
plt.figure(figsize=(12,6))
plt.plot(years, oranges, marker='o',label='oranges')
plt.title("yield of oranges (tons per hectare)")
plt.legend()
```
<img width="1127" height="732" alt="image" src="https://github.com/user-attachments/assets/6a4b33f1-066e-41c4-b714-53cd8f6a0f7c" />

```
import matplotlib.pyplot as plt
print("scatter plot is:")
x = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]
plt.scatter(x, y, label='star', color='green', marker='*', s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```
<img width="728" height="773" alt="image" src="https://github.com/user-attachments/assets/1f8cb7ed-e791-4539-ab0c-18f1b56abfe3" />

```
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='green',label='y1')
plt.fill_between(x, y2, color='blue', label='y2')
plt.fill_between(x, y3, color='red',label='y3')
plt.title("Fill Between Example")
plt.legend()
plt.show()
```
<img width="722" height="740" alt="image" src="https://github.com/user-attachments/assets/5c4a4c49-f7d2-4a38-b58f-76daeb00ce46" />

```
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
<img width="648" height="660" alt="image" src="https://github.com/user-attachments/assets/ebc08f06-be11-4ee1-af83-970a2d9557ca" />

```
from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 9, 10, 11, 12, 13])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.show()
```
<img width="627" height="686" alt="image" src="https://github.com/user-attachments/assets/e9605284-ce0b-4485-b026-dbaf56ba849a" />

```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```
<img width="696" height="577" alt="image" src="https://github.com/user-attachments/assets/c93a2c6f-b2ec-4097-b06c-14b2b81bd437" />

```
ages = [2, 5, 70, 40, 45, 50, 43, 40, 44, 60, 7, 13, 57, 18, 90, 77, 32, 21, 20, 40]
range1 = (0, 100)
bins = 10
plt.hist(ages, bins, range1, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no. of people')
plt.title('my histogram')
plt.show()
```
<img width="754" height="681" alt="image" src="https://github.com/user-attachments/assets/60e21cea-394f-4184-b924-0ac8bf8871f3" />


```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()
```
<img width="671" height="557" alt="image" src="https://github.com/user-attachments/assets/11c5eb10-8bcc-4713-b9e4-2393fed8b6c2" />

```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
<img width="686" height="482" alt="image" src="https://github.com/user-attachments/assets/56d3cac9-7a71-47e4-9108-1f9b1b5ad549" />

```
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```
<img width="706" height="670" alt="image" src="https://github.com/user-attachments/assets/d4d630ff-9615-4e5b-b8a1-583fd95e9fcd" />

```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6]
colors=['y', 'g', 'b', 'r']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0), radius=1.2, autopct="X1.1")
plt.legend()
plt.show()
```
<img width="1129" height="596" alt="image" src="https://github.com/user-attachments/assets/4099111c-471d-4567-849e-ad9b60792397" />

```
labels='python', 'C+', 'ruby', 'java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```
<img width="832" height="603" alt="image" src="https://github.com/user-attachments/assets/733e4be9-7c83-4c2f-9891-395c95f97d03" />


# Result:
 Result is successfully executed
