# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1) Start the program
2) Import the necessary libraries(numpy,scipy.linalg)
3) Define the matrix using numpy
4) Use lu(),lu_solve(),lu_factor() to get the solutions
5) End the program

## Program:
(i) To find the L and U matrix
```
Program to find L and U matrix using LU decomposition.
Developed by: Thaarakeshwar
RegisterNumber:  212225040466
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()), dtype=float)
P, L, U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
Program to find L and U matrix using LU decomposition.
Developed by: Thaarakeshwar
RegisterNumber:  212225040466
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()), dtype=float)
b = np.array(eval(input()), dtype=float)
lu, piv = lu_factor(A)
x = lu_solve((lu, piv), b)
print(x)
```
## Output:

<img width="1012" height="483" alt="image" src="https://github.com/user-attachments/assets/65890649-cab8-478a-af51-5a35bd4cb8d4" />

<img width="1012" height="273" alt="image" src="https://github.com/user-attachments/assets/54f9fa8f-d108-4c09-a1ca-76f190319c13" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

