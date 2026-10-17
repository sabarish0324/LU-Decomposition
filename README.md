# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: SABARISHWARAR S.P
RegisterNumber: 26010660
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: 
RegisterNumber: 
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:
<img width="1393" height="841" alt="image" src="https://github.com/user-attachments/assets/d6cbf7b7-bca6-4077-9ccb-33a3df0563c1" />
<img width="1205" height="553" alt="image" src="https://github.com/user-attachments/assets/938970a6-d815-42bd-b8d3-963bbf743296" />
<img width="1188" height="697" alt="image" src="https://github.com/user-attachments/assets/6023797e-73a1-41f6-97fd-4e8dd998ff2f" />
<img width="1222" height="290" alt="image" src="https://github.com/user-attachments/assets/5f810c3f-5c4d-400c-b5f3-2dd7f5507eda" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

