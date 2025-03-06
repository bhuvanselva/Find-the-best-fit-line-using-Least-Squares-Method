# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 

![image](https://github.com/user-attachments/assets/464ecfa0-8d5c-4060-a83f-520bf701b0bc)


4. Compute the y -intercept of the line by using the formula:

![image](https://github.com/user-attachments/assets/a98f3c6a-98b3-46a6-907b-ce78457c763d)

5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: BHUVANESHWARI S
RegisterNumber: 212222220008

import numpy as np
import matplotlib.pyplot as plt

X=np.array(eval(input()))
Y=np.array(eval(input()))

X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0

for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denom+=(X[i]-X_mean)**2

m=num/denom

b=Y_mean-m*X_mean

print(m,b)

y_predicted=m*X+b
print(y_predicted)

plt.scatter(X,Y)
plt.plot(X,y_predicted,color='red')
plt.show()
*/


## Output:
![image](https://github.com/user-attachments/assets/c538e6ef-16a2-4b8b-9aea-44d29ce0ffaf)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
