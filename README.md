# Norm of a matrix
## Aim
To write a program to find the 1-norm, 2-norm and infinity norm of the matrix and display the result in two decimal places.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
	1. Get the input matrix using np.array()   
    2. Find the 2-norm of the matrix using np.linalg.norm()
	3. Print the norm of the matrix in two decimal places.
## Program:
```Python
#Developed by: G.Sanjay
#RegisterNumber: 212224230243
# 1-Norm of a Matrix

#EXP.7-CR-Norm of a matrix
##NAME:G.Sanjay
##REG.NO:212224230243

import numpy as np
def one_norm(matrix):
    arr = np.array(matrix)
    norm_value = np.linalg.norm(arr, 1)  # 1-Norm (column-wise maximum absolute sum)
    return norm_value
matrix =eval(input())
result = one_norm(matrix)
print(f"{result:.2f}")
# 2-Norm of a Matrix
'''
Program to find 2-norm of a matrix.
Developed by: G.Sanjay
RegisterNumber: 212224230243
'''
import math
import numpy as np
def l2_norm(matrix):
    A = np.array(matrix, dtype=float)
    return np.linalg.norm(A, 2)
mat1 = eval(input())
print(f"{l2_norm(mat1):.2f}")

# Infinity Norm of a Matrix
'''
Developed by: G.Sanjay
RegisterNumber: 212224230243
'''
def infinity_norm(matrix):
   
    row_sums = [sum(abs(val) for val in row) for row in matrix]
    return max(row_sums)
mat =eval(input())
print(f"{infinity_norm(mat):.2f}")  # 8.00

```
## Output:
### 1-Norm of a Matrix
![WhatsApp Image 2025-11-26 at 9 44 10 PM](https://github.com/user-attachments/assets/cdf44c69-fdc0-4c5d-a844-776a68334915)


### 2-Norm of a Matrix
![WhatsApp Image 2025-11-26 at 9 44 23 PM](https://github.com/user-attachments/assets/4b61aa83-0912-4b98-91ee-4f29838f6894)


### Infinity Norm of a Matrix
![WhatsApp Image 2025-11-26 at 9 44 36 PM](https://github.com/user-attachments/assets/c4a2f7b4-3637-40d4-ae07-f6ae5a0108c5)


## Result
Thus the program for 1-norm, 2-norm and Infinity norm of a matrix are written and verified.
