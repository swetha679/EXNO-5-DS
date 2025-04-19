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
REG NO:212224040345
NAME:B R SWETHA NIVASINI
```


# LINE GRAPHS:

```
import matplotlib.pyplot as plt
x_val = [0,1,2,3,4,5]
y_val = [0,1,4,9,16,25]
plt.plot(x_val,y_val)
plt.show()
```

![Screenshot 2025-04-19 115058](https://github.com/user-attachments/assets/d1d34e6a-b0ce-4c4b-bcbd-442bf00b7d60)

```
import matplotlib.pyplot as plt
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('GRAPH-1')
plt.show()
```
![Screenshot 2025-04-19 115149](https://github.com/user-attachments/assets/a6369b0f-5f14-46ad-aeaa-0108ecc641de)

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,4,1]
plt.plot(x1,y1,label = 'line 1')
x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x2,y2,label = 'line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines in the Same Graph")
plt.legend()
plt.show()
```
![Screenshot 2025-04-19 115227](https://github.com/user-attachments/assets/51a145ca-d603-4d54-bca2-001e6138cfd6)

```
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]

plt.plot(x,y, color='green', linewidth=3, linestyle='--', marker = '*', markerfacecolor='orange', markersize=10)
plt.ylim(1, 8)
plt.xlim(1, 8)
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.title("Dotted Line")
plt.show()
```

![Screenshot 2025-04-19 115302](https://github.com/user-attachments/assets/2aa9ffa9-29d0-4161-89ab-6c26adce7b2b)

```
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6]
y = [2, 4, 1, 5, 2, 6]
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*--')
plt.subplot(2,2,3)
plt.plot(x,x,'bo--')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![Screenshot 2025-04-19 115337](https://github.com/user-attachments/assets/aa33c264-535c-4da0-87d7-169a5480822b)


# SINE WAVE FORM:

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
np.pi
x=np.arange(0,3*np.pi,0.1)
y=np.sin(x)
plt.title("SINUSOIDAL WAVE")
plt.plot(x,y)
plt.show()
```

![Screenshot 2025-04-19 115416](https://github.com/user-attachments/assets/d2fafdb5-59fa-4f2f-99ad-ab618644f2cd)


```
import matplotlib.pyplot as plt

x_values = [0, 1, 2, 3, 4, 5]
y_values = [0, 1, 4, 9, 16, 25]

plt.scatter(x_values, y_values, s=30, color="red")
plt.show()
```
![Screenshot 2025-04-19 115456](https://github.com/user-attachments/assets/da3a08d8-43c8-46b2-991a-6deebd16f292)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]

plt.fill_between(x,y1,color="pink")
plt.legend(['y1'])
plt.show()
```
![Screenshot 2025-04-19 115549](https://github.com/user-attachments/assets/12d915e2-ab5a-49ee-ad5e-cc2275d1d734)

```
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.stackplot(x,y1,y2,y3,labels = ['Y1','Y2','Y3'])
plt.legend(loc = 'upper left')
plt.title('Stacked AREA Chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

![Screenshot 2025-04-19 115629](https://github.com/user-attachments/assets/3002db28-65af-4609-8b0a-7577da141058)

```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 8, 9, 10, 11, 12])
x_smooth = np.linspace(x.min(), x.max(), 300)
spline = make_interp_spline(x, y)
y_smooth = spline(x_smooth)
plt.figure(figsize=(8, 5))
plt.plot(x, y, 'o', label='Original Data')
plt.plot(x_smooth, y_smooth, label='Cubic Spline Interpolation')
plt.title("Cubic Spline Interpolation")
plt.xlabel("X-AXIS")
plt.ylabel("Y-AXIS")
plt.legend()
plt.show()
```

![Screenshot 2025-04-19 115710](https://github.com/user-attachments/assets/94cbd341-3f79-4e73-8d71-f0910af96124)

```
import numpy as np
import matplotlib.pyplot as plt
val = [5, 6, 3, 7, 2]
names  = ["A", "B", "C", "D", "E"]
plt.bar(names, val,color = 'pink')
plt.show()
```

![Screenshot 2025-04-19 115748](https://github.com/user-attachments/assets/6958da2b-5521-4271-931c-0908adbdb32e)

```
import matplotlib.pyplot as plt
values = [5, 6, 3, 7, 2]
names  = ["A", "B", "C", "D", "E"]
colors = ['b', 'g', 'b', 'g', 'b']
plt.figure(figsize=(8, 5))
plt.bar(names, values, color=colors)
plt.title("Bar Chart")
plt.xlabel("Categories")
plt.ylabel("Values")
plt.tight_layout()
plt.show()
```

![Screenshot 2025-04-19 115819](https://github.com/user-attachments/assets/2ec14715-fccc-4138-83f2-1398a78cb64e)

```
import matplotlib.pyplot as plt

x = [2, 8, 10]
y = [11, 16, 9]
x2 = [3, 9, 11]
y2 = [6, 15, 7]

plt.bar(x,y,color="r")
plt.bar(x2,y2,color="b")
plt.title("Bar graph for 2 features")
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![Screenshot 2025-04-19 115913](https://github.com/user-attachments/assets/7c0fd16d-612b-4e6b-a8d5-8e2f39c49e41)

```
import matplotlib.pyplot as plt
import numpy as np
ages = [2,6,4,12,13,12,16,18,18,19,26,24,39,34,45,42,54,56,90,56,86,79]
range = (0,100)
bins = 10
plt.hist(ages,bins,range,color='brown',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```

![Screenshot 2025-04-19 115952](https://github.com/user-attachments/assets/ea0b71a8-c04f-42d5-a2a5-23b068ebb932)


```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2025-04-19 120030](https://github.com/user-attachments/assets/f73f534e-2e7e-4150-9158-6e9ebd8714c1)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![Screenshot 2025-04-19 120102](https://github.com/user-attachments/assets/d588fe20-8427-4d81-947d-f273a60bdbdd)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

![Screenshot 2025-04-19 120145](https://github.com/user-attachments/assets/f68447dc-b996-435c-984a-905e75817fc4)



# Result:
 Thus the data visualization using matplot python library for the given datas are performed successfully.
