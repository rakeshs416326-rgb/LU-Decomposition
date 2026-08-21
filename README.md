# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm (i): To find L and U matrices
Step 1: Start the program.
Step 2: Import required libraries (numpy and scipy.linalg).
Step 3: Read the input square matrix using numpy.array().
Step 4: Apply lu() function to decompose the matrix into P, L, and U.
Step 5: Extract L (Lower triangular matrix) and U (Upper triangular matrix).
Step 6: Display L matrix.
Step 7: Display U matrix.
Step 8: Stop the program.

## Algorithm (ii): To solve using LU Decomposition
Step 1: Start the program.
Step 2: Import required libraries (numpy and scipy.linalg).
Step 3: Read the coefficient matrix using numpy.array().
Step 4: Read the constant matrix (right-hand side values).
Step 5: Apply lu_factor() to factorize the matrix into LU form.
Step 6: Apply lu_solve() using the LU factors and constants.
Step 7: Display the solution vector. Step 8: Stop the program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Rakesh s
RegisterNumber: 212225240114
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Rakesh S
RegisterNumber: 212225240114

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)
*/
```

## Output:
<img width="1047" height="419" alt="image" src="https://github.com/user-attachments/assets/cbb6a46c-cc82-4b1d-8bde-36f1e0f75883" />
<img width="1052" height="244" alt="image" src="https://github.com/user-attachments/assets/8049cf0d-afef-4aaf-81cd-263217399d9f" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

