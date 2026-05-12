# RANK-OF-A-MATRIX
## Aim:
To write a python program to find the rank of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step 1: start the program
### Step 2: use math function
### Step 3: Using the np.linalg.matrix_rank(), we can find the rank of the given matrix.
### Step 4: end program

## Program:

```
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
A = np.array([[1, 2, 3],[3, 6, 9]])
rank = np.linalg.matrix_rank(A)
print(rank)

```

## Output:

<img width="1482" height="912" alt="image" src="https://github.com/user-attachments/assets/13326396-40e6-4b6b-8764-b4588484caa5" />


## Result:
Thus the rank for the given matrix is successfully solved by  using a python program.

