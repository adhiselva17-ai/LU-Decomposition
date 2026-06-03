# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Write a python program for the given matrix. 2.Using numpy library. 3.Using the np.linalg.matrix_rank(),we can find the rank of the matrix. 4.Run the program and get the output. 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: ADHI SELVAKUMAR R
RegisterNumber: 212225220003
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
P,L,U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: ADHI SELVAKUMAR R
RegisterNumber: 212225220003
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array([[3,2,7],[2,3,1,],[3,4,1]])
B=np.array([4,5,7])
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)



```

## Output:
<img width="830" height="883" alt="Screenshot 2026-06-02 200324" src="https://github.com/user-attachments/assets/58a124ed-5c5e-4f92-a56e-f20622aa86d3" />
<img width="1291" height="461" alt="Screenshot 2026-06-02 200344" src="https://github.com/user-attachments/assets/ce42e7e7-0e71-4b3a-8e71-538c3003a780" />
<img width="949" height="732" alt="Screenshot 2026-06-02 200357" src="https://github.com/user-attachments/assets/3f6b0564-d8b4-4057-bc74-94bea8809c9d" />
<img width="1146" height="227" alt="Screenshot 2026-06-02 200413" src="https://github.com/user-attachments/assets/d2f2e27b-023e-4ef8-8a37-4c17d3b81245" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

