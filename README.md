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
#Univariate Linear Regression
#Developed by: THEJASWINI
#Reference number: 212223110059
import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.scatter(x,ypred,color="Blue")
plt.show()






```
## Output
![Screenshot 2023-12-31 133433](https://github.com/thejaswinidhanaraj/Univariate-Linear-Regression/assets/148514511/7591ef15-bde7-4e31-ab05-891fbe6e02f1)
![Screenshot 2023-12-31 133508](https://github.com/thejaswinidhanaraj/Univariate-Linear-Regression/assets/148514511/1f2f1889-2d08-4e04-9020-868434bbd4b2)
![Screenshot 2023-12-31 133604](https://github.com/thejaswinidhanaraj/Univariate-Linear-Regression/assets/148514511/47b832c2-fb53-469c-b621-1279c7bc52e6)


</br>
</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
