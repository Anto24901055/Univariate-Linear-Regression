# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: ANTO WILLIAMS S
RegisterNumber: 24901055
*/

import numpy as np
from matplotlib import pyplot
x=np.array(eval(input()))
y=np.array(eval(input()))
Xmean=np.mean(x)
Ymean=np.mean(y)
num,den=0,0
for i in range(len(x)):
    num+=(x[i]-Xmean)*(y[i]-Ymean)
    den+=(x[i]-Xmean)**2
slope=num/den
c=Ymean-slope*Xmean
y_per=slope*x+c
pyplot.scatter(x,y,color='blue')
pyplot.plot(x,y_per,color='black')
pyplot.show()



```
## Output
![Screenshot 2024-12-26 214924](https://github.com/user-attachments/assets/10d595bb-2f7f-4649-86ce-854e7c190330)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
