## NAME: PRAISY NISHITHA J
## REGISTER NUMBER : 212224100042

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Input the coefficient matrix A and the constant vector B (if solving equations).

Step 2: Perform LU decomposition of matrix A to obtain:

L → Lower triangular matrix

U → Upper triangular matrix

P → Permutation matrix (if required)

Step 3:

If solving equations: use the LU factors to solve for X in 
𝐴
𝑋
=
𝐵
AX=B.

If analyzing only: display the L and U matrices.

Step 4: Output the result:

Solution vector X (for system solving), or

Matrices L and U (for decomposition display).

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
(ii) To find the LU Decomposition of a matrix
```
```
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:

<img width="1464" height="826" alt="image" src="https://github.com/user-attachments/assets/13303024-7a60-4486-86bc-4b321ca79b68" />

<img width="1467" height="645" alt="image" src="https://github.com/user-attachments/assets/18c87f97-a522-4611-a6a6-a36cd30ac74b" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

