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

import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/c66f5c32-89e6-4b10-b7a7-71af59e2c247)

import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/a608dd72-b67b-4022-aa78-371b1619d43c)

yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/a00621d6-3311-4fa2-acf5-391c2acd66cf)

years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/5dee0bba-9ea2-45c8-98f9-4d07e83cc8b7)

years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/6012f3f0-6f87-4cf8-bd6e-5ba507a1b06d)

plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/bb1912de-70f1-4707-b42c-360d1d3fe09f)

import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/f13513f0-5c94-4933-864e-287b241a7927)

y

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/a870782e-3cd4-4d44-a653-4ab7cd289888)

plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/d201a979-810e-4735-a49c-8ef3c57f6a74)

y=x*x
y

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/809779da-a186-4e40-b85b-2760598b20b9)

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/d7751af4-13ae-490a-a352-4ab023c36fc1)

np.pi

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/d8c70094-b994-4503-9832-4fba61e65f9a)

x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/57d1482c-2b3b-4a7c-9cf8-12980dd73b17)

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/6f1efd80-4e8d-45bb-bd8a-97e7cfeac3bd)

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/3dee5ad9-ae9e-4bab-9112-ecb29018bc9e)

import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/1e1a02fb-7398-44e6-b06e-35c1db335bb0)

x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/2631e29c-cc9b-4d12-9f07-0bd21b2b9db5)

import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/0c306853-c5be-4dca-a879-0dfc4a30bff8)

import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/70bf4782-2179-44ea-aa7d-7dba6eebf101)

fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/0f940dad-69e3-4c11-bca0-838d3c32ea79)

labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/04c6c150-926c-4f18-adf4-cf8273c26d01)

activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()

![image](https://github.com/22008650/EXNO-5-DS/assets/122548204/ecf37e01-15ea-4221-bc99-df88d93bdcb3)

# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
