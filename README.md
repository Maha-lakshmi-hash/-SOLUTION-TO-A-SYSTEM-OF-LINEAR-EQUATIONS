# -SOLUTION-TO-A-SYSTEM-OF-LINEAR-EQUATIONS
## Aim:
To write a python program to find a solution to a system of linear equations.
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3: 
Using the np.linalg.solve(), we can find the solutions.
### Step 4: 
End the program
## Program:
```
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"

matrix = eval(input())

rows = len(matrix)
cols = len(matrix[0])

max_sum = 0

for j in range(cols):
    col_sum = 0
    for i in range(rows):
         col_sum += abs(matrix[i][j])
    
    if col_sum > max_sum:
        max_sum = col_sum
        
print(f"{max_sum:.2f}")
'''
Program to find 2-norm of a matrix.
Developed by: Maha Lakhsmi K
RegisterNumber: 212225040220
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np

matrix = eval(input())

A = np.array(matrix)

norm = np.linalg.norm(A, 2)

print(f"{norm:.2f}")
import os

os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np

matrix =  eval(input())

A = np.array(matrix)

norm = np.linalg.norm(A, np.inf)

print(f"{norm:.2f}")
```

## Output:

<img width="1920" height="1080" alt="Screenshot 2026-05-29 100845" src="https://github.com/user-attachments/assets/55f727d7-2f67-40ef-ba5a-3637529b42c9" />


<img width="1920" height="1079" alt="Screenshot 2026-05-29 101100" src="https://github.com/user-attachments/assets/ce6fb2bf-b952-403c-9fd8-f46418f4d833" />


<img width="1920" height="1080" alt="Screenshot 2026-05-29 101111" src="https://github.com/user-attachments/assets/f5c30577-f3fc-4118-af3e-5ca694058582" />


## Result: 
Thus the solutions for the linear equations are successfully solved using python program

