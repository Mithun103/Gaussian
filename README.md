# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import numpy from the Python libraray.
2.Get the matrix input from the user.
3.Calculate the variable using libraries.
4.Print the result.
5.End the program.

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: mithun ms
RegisterNumber: 22008364
import numpy as np
n=int(input())
ar=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        ar[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=ar[j][i]/ar[i][i]
        for k in range(n+1):
            ar[j][k]=ar[j][k]-ratio*ar[i][k]
x[n-1]=ar[n-1][n]/ar[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=ar[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-ar[i][j]*x[j]
    x[i]=x[i]/ar[i][i]
for i in range(n):
    print("X%d = %0.2f"%(i,x[i]),end=" ")
*/
```

## Output:



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

