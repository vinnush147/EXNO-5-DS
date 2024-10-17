EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
Aim:
To Perform Data Visualization using matplot python library for the given datas.

EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

Coding and Output:
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
y
326245288-1cd7f531-6748-4b3a-a86c-b183341dfbd7

326245299-d70b19e5-7476-4d5d-9cc3-3ba1cb99ed63

x=np.arange(40,50)
y=np.arange(50,60)
x
y
326248396-d069289a-f353-488e-9591-e2cbb70f66b8

326248398-c7e89fa4-0c57-454b-9c37-1a235581fa88

#Scatterplot
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
326248475-f8d03027-984e-4c93-bea8-61e862e983e5

y=x*x
y
326248503-508e913d-45aa-4019-ac6e-3bb0957e41dc

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2D Diagram')
326248542-945fac89-77f2-4d35-b687-d9de408f2808

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2D Diagram')
326248542-945fac89-77f2-4d35-b687-d9de408f2808

plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
326248570-e31f9ae1-743f-40ab-8981-0757507e1d5d

# Compute the x and y coordinates for points on a
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")

#Plot the points using matplotlib
plt.plot(x,y)
plt.show()
326248612-be5de64e-2fd5-492d-bc12-d28ca4ceebc7

#BAR Chart
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.show()
326248661-97242f80-31f8-4e5b-9515-ec704c4ac331

x=np.arange(1,11)
y=3*x+5
plt.title("Matplotlib demo")
plt.xlabel("x axis caption")
plt.ylabel("y axis caption")
plt.plot(x,y)
plt.show()
326249440-3eab5f54-0b3b-4a80-9a6b-1674989d2ac2

x=np.arange(0,5 *np.pi,0.1)
y_sin=np.sin(x)
y_cos=np.cos(x)
plt.subplot(2,1,1)
plt.plot(x,y_sin,'r--')
plt.title('Sine')
plt.subplot(2,1,2)
plt.plot(x,y_cos,'g--')
plt.title('Cosine')
plt.show()
326249475-ff7eaad8-2fbf-4679-bea3-197ffc921d14

a=np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27])
plt.hist(a,color='g')
plt.title("histogram")
plt.show()
326249537-609c39c2-e5bb-4251-8103-b87736ca3c27

labels=['A','B','C']
values=[1,4,2]
plt.figure(figsize=(5,3),dpi=100)
bars=plt.bar(labels,values,color='green')
patterns=['-','*','+']
for bar in bars:
  bar.set_hatch(patterns.pop(0))
plt.savefig('barchat.png',dpi=100)
plt.show()
326249580-8ee09a70-3dff-4eb0-88dc-59afafee371b

import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
326249699-9ef8f0c2-7455-495e-bd44-59222291a5da

import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph!')
plt.show()
326249724-f31c88a6-6028-4dcb-a1c8-4fbbbfb970d1

import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
plt.show()
326249793-91acd162-fd82-463e-84d8-687aef9ad3b6

import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,
         marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
plt.show()
326249835-942335fb-50b9-4f75-8589-ac2b8e4a042a

yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
326249859-8e8a7101-671b-4ccd-b0d1-5504f1fdf34d

years=[2010,2011,2012,2013,2014,2015]
yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
326249905-2df6d348-97d6-4fa8-a1c2-b01aff92c891

years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.900,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel("year")
plt.ylabel("Yield(toes per hectare)");
326249939-7e3d05ad-a32f-4763-93eb-3fe121805d66

plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (toes per hectare)");
326250001-32d91b16-1963-4e74-92ce-a428f84350dc

plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges'])
326250041-f7575df2-644c-4b25-8602-12bcc13c2558

import matplotlib.pyplot as plt
x_values = [1,2,3,4,5,6,7,8,9,10]
y_values = [2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="stars",color="blue",marker="*",s=30)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("My scatter plot!")
plt.legend()
plt.show()
326250082-b8c7e7e9-7764-47d4-bfde-f8e5d3517dcb

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="blue")
plt.fill_between(x,y2,color="green")
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
326250151-c2323a0c-e924-42f3-925a-d2781f912390

x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2','Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
326250189-a7b871ab-91e0-4bdb-bfa3-ab08c529cbb6

import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x = np.array([1,2,3,4,5,6,7,8,9,10])
y = np.array([2,4,5,6,7,8,8,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='spline')
plt.legend()
plt.show()
326250262-e66e9a37-73d8-4deb-8479-8ce4e0958559

Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
