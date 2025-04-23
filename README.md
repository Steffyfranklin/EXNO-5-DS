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
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.plot(x,y)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.show()
```
![image](https://github.com/user-attachments/assets/7967ef4e-4e31-4b1f-a4e6-827ac911fa18)
```
x1=[1,2,3]
y1=[2,4,1]
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.plot(x1,y1,label="line 1")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/e645257c-0351-4a8a-b057-4abfb0a4fd59)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color="blue",linewidth=9,linestyle="dashed",marker='o',markerfacecolor='red',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH")
plt.show()
```
![image](https://github.com/user-attachments/assets/11da38ee-55ec-4e4d-bb0c-c4ba99e04016)
```
years=range(2000, 2012)
apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375,0.9372,0.939]
oranges=[0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898,0.9,0.896]

plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/user-attachments/assets/cdfd0c75-6e3f-486c-8fab-ad6aff32e1fc)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/6fc516e7-dd1a-4c3b-ad66-497b3555a944)
```
years = [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples)
plt.xlabel('YEAR')
plt.ylabel('YIELD(tons per hectare)')
```
![image](https://github.com/user-attachments/assets/38aa9e96-196a-45ba-a929-f4340cb6f066)
```
plt.figure(figsize=(10,6))
y=list(range(2000,2012))
plt.plot(y,oranges,marker='o')
plt.title("YIELD OF ORANGES(tons per hectare)")
```
![image](https://github.com/user-attachments/assets/0780b947-d2c4-4f32-b188-1f4e8934dd68)
```
plt.plot(y,oranges,marker='x')
plt.plot(y,apples,marker='o')
plt.xlabel("YEAR")
plt.ylabel("YIELD(tons per hectare)")
plt.title("YIELD OF ORANGES AND APPLES(tons per hectare)")
plt.legend(["oranges","apples"])
```
![image](https://github.com/user-attachments/assets/93a8322c-3c81-4bc0-ac6a-83d117b81a65)
```
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.scatter(x,y,s=30,color="blue")
plt.show()
```
![image](https://github.com/user-attachments/assets/2f761a1a-06be-4993-85b0-8b2d17ea32e9)
```
x=[0,1,2,3,4,5]
y=[10,20,4,16,30,40]
plt.scatter(x,y,marker="*",color="black")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("SCATTER PLOT")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/e3cc6f16-5e6e-4e59-a467-f6c4fc0d14b4)
```
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/9acf372b-fda8-43f9-aacc-0ad6fcf37f1c)
```
y
```
![image](https://github.com/user-attachments/assets/ca6b0318-16bb-45ec-ab17-0a2633b08df4)
```
plt.scatter(x,y,c="r")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("GRAPH IN 2D")
plt.savefig("Test.png")
```
![image](https://github.com/user-attachments/assets/e826c780-d984-48dc-921c-167ea27c0a09)
```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/1d33f808-5996-4bd4-977c-1642eb2040be)
```
plt.plot(x,y,'g*',linestyle="dashed",linewidth=2,markersize=12)
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.title("2D GRAPH")
```
![image](https://github.com/user-attachments/assets/73bc46da-6c7f-40e4-b773-cc88d6c6b26e)
```
plt.subplot(2, 2, 1)
plt.plot(x, y, 'r--')
plt.subplot(2, 2, 2)
plt.plot(x, y, 'g*--')
plt.subplot(2, 2, 3)
plt.plot(x, y, 'bo')
plt.subplot(2, 2, 4)
plt.plot(x, y, 'go')
```
![image](https://github.com/user-attachments/assets/a5db35c0-2492-4261-af55-61541277c382)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x, y)
plt.show()
```
![image](https://github.com/user-attachments/assets/e984df24-dfb7-45fb-9075-263eb459bfa7)
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2=[5, 7, 9, 11, 13]
y3=[2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='purple')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/945dc0b2-fbae-416d-a0e9-651f9eb8ae33)
```
plt.stackplot(x, y1, y2, y3, labels=['Line 1', 'Line 2', 'Line 3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/e99e8b1b-3124-4aa4-92b9-4d924a71763a)
```
from scipy.interpolate import make_interp_spline
x= np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 8, 9, 10, 11, 12])

spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.title("SPLINE CHART")
plt.show()
```
![image](https://github.com/user-attachments/assets/99d67a16-845d-403e-a7d4-1d156862165a)
```
val=[5,4,8,6,3]
names=["A","B","C","D","E"]
plt.bar(names,val,color="blue")
plt.title("BAR GRAPH")
plt.show()
```
![image](https://github.com/user-attachments/assets/93c4a47a-f1d3-4587-9901-39936d08e4b5)
```
plt.barh(names,val,color="pink")
plt.title("BAR GRAPH(horizontal)")
plt.show()
```
![image](https://github.com/user-attachments/assets/8dc066be-70c1-4f95-b97f-5642d9067873)
```
height=[10,24,36,37,45]
names=['one','two','three','four','five']
c1=['green','blue']
c2=['b','g']
plt.bar(names,height,color=c1,width=0.8)
plt.xlabel("names")
plt.ylabel("height")
plt.title("BAR CHART")
plt.show()
```
![image](https://github.com/user-attachments/assets/e99a3818-c73b-4a10-b29a-a245394c4e5e)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x, y,color='red')
plt.bar(x2, y2, color = 'purple')
plt.title("Bar graph")
plt.ylabel('Y axis')
plt.xlabel('x axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/75344ca7-1227-40a3-aa41-7e5e1bfad487)
```
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0, 100)
bins=10
plt.hist(ages, bins, range, color='cyan', histtype='bar', rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('Histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/a2a56150-e1b9-403f-8ad5-4c3191ef7969)
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins=10, color='blue', alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/43db43c0-ac5f-433e-9f2e-45b0a99ef4f7)
```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/18bc0f6e-c635-4ecf-9a0d-af8d089ac1df)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_title("BOX PLOT")
ax.set_ylabel("Y-AXIS")
ax.set_xlabel("X-AXIS")
```
![image](https://github.com/user-attachments/assets/56ae2ab2-d3ba-49d1-9709-addf26adda8f)
```
activities = ['eat', 'sleep', 'work', 'play']
slices=[3, 7, 8, 6]
colors = ['r', 'y', 'g', 'b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0), radius=1.2, autopct='%1.1f%%')
plt.legend ()
plt.show()
```
![image](https://github.com/user-attachments/assets/61547b1c-12ff-4062-a11f-13add01136bb)
```
labels=['Python','C++','Ruby','Java']
sizes=[215, 130, 245, 210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/6aeb8aeb-769d-490c-884d-db5b74569223)

# Result:
      Successfully Perform Data Visualization using matplot python library for the given datas.
