# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
```
Step 1: Input the matrix A from the user.
Step 2: Perform LU decomposition on A to obtain P, L, U such that PA = LU.
Step 3: Extract the lower triangular matrix L and upper triangular matrix U.
Step 4: Print the matrices L and U.

(ii)
Step 1: Input the matrix A and the vector b from the user.
Step 2: Compute the LU factorization of A using lu_factor to get lu and piv.
Step 3: Solve the system AX = b by applying lu_solve with the LU factors and pivots.
Step 4: Print the solution vector X.  
```

## Program:
(i) To find the L and U matrix
```

Program to find the L and U matrix.
Developed by: V PATRICK ALEX EMMANUEL
RegisterNumber: 212224240110

import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```

Program to find the LU Decomposition of a matrix.
Developed by: V PATRICK ALEX EMMANUEL
RegisterNumber: 212224240110

import numpy as np
from scipy.linalg import lu,solve_triangular
a=np.array(eval(input()))
b=np.array(eval(input()))
p,l,u=lu(a)
pb=np.dot(p,b)
y=solve_triangular(l,pb,lower=True)
x=solve_triangular(u,y)
print(x)
```

## Output:
1)
<img width="895" alt="Screenshot 2025-05-22 at 11 06 05 AM" src="https://github.com/user-attachments/assets/fcb6ae62-621f-4008-b972-67865f24d368" />

2)
<img width="746" alt="Screenshot 2025-05-22 at 11 06 25 AM" src="https://github.com/user-attachments/assets/60f4cbd0-7793-4209-9ac3-9b3390442d0f" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

