# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

Step 1:
Import required libraries numpy and scipy.linalg.

Step 2:
Input the matrix/matrices using eval(input()).

Step 3:
Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().

Step 4:
Print the results L and U matrices or solution X matrix

## Program:
(i) To find the L and U matrix
```
'''
Program to find L and U matrix using LU decomposition.
Developed by: VISWAJITH LALITHRAM R.V
RegisterNumber: 212224240187


'''

import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: VISWAJITH LALITHRAM R.V
RegisterNumber: 212224240187

'''

# To print X matrix (solution to the equations)

import numpy as np
from scipy import linalg
A = np.array([[3,2,7], [2,3,1], [3,4,1]])
B = np.array([4,5,7])
P, L, U = linalg.lu(A)
Y = np.linalg.solve(L, np.dot(P, B))
X = np.linalg.solve(U, Y)
print(X)
```

## Output:
(i)

<img width="986" height="806" alt="Screenshot 2025-08-28 094328" src="https://github.com/user-attachments/assets/d92237d4-6dd4-4d4a-a200-e95d8759d574" />

(ii)

<img width="717" height="597" alt="Screenshot 2025-08-28 094313" src="https://github.com/user-attachments/assets/da3faac4-308a-401a-b4a2-9837a4f9c860" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

