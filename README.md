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
x_val = [0,1,2,3,4,5]
y_val = [0,1,4,9,16,25]
plt.plot(x_val,y_val)
plt.show()
```
![image](https://github.com/user-attachments/assets/3a5f9d07-34f7-43de-b661-0fbea6430a09)

```
import matplotlib.pyplot as plt
x = [1,2,3]
y = [2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
![image](https://github.com/user-attachments/assets/36ff16b0-99ab-469d-9ba1-ba7504b352eb)

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,5,3]
plt.plot(x1,y1,label = 'line 1')
x2 = [1,2,3]
y2 = [3,1,6]
plt.plot(x2,y2,label = 'line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/9a02069b-3acb-49fd-92fa-f37f273ca781)

```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x,y1,color = 'blue')
plt.fill_between(x,y2,color = 'orange')
```
![image](https://github.com/user-attachments/assets/5a4c2cb5-c286-4c3f-9a7f-0d74658b810b)

```
plt.stackplot(x,y1,y2,y3,labels = ['line1','line2','line3'])
plt.legend(loc = 'upper left')
plt.title('Stacked line charts')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/aaad0e37-31d5-4f60-9dc7-bf8d9b61a4af)

```
import numpy as np
import matplotlib.pyplot as plt
val = [2,4,7,3]
names = ['A','B','C','D']
plt.bar(names, val,color = 'purple')
plt.show()
```
![image](https://github.com/user-attachments/assets/f620142b-8c2b-4ef4-9448-a99049ea648b)

```
import matplotlib.pyplot as plt
import numpy as np
ages = [2,6,4,12,13,12,16,18,18,19,26,24,39,34,45,42,54,56,90,56,86,79]
range = (0,100)
bins = 10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/6b03870c-224e-4f9b-8903-900fd3bc3cb7)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data                         
```
![image](https://github.com/user-attachments/assets/6d6f0048-bc8e-49cf-8dc8-509804889bff)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![image](https://github.com/user-attachments/assets/6c8d1a07-58a2-44f4-914c-564242d61000)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = 
(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/5ac2281b-2e78-4f48-b049-c4c0133152aa)

# Result:
Thus the program is executed successfully.
