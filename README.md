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
def matrix_rank(A):
    A = [list(map(float, row)) for row in A]
    m, n = len(A), len(A[0])
    rank = 0

    for col in range(n):
        pivot = None
        for row in range(rank, m):
            if abs(A[row][col]) > 1e-10:
                pivot = row
                break

        if pivot is None:
            continue

        A[rank], A[pivot] = A[pivot], A[rank]

        pivot_val = A[rank][col]
        for j in range(col, n):
            A[rank][j] /= pivot_val

        for i in range(m):
            if i != rank:
                factor = A[i][col]
                for j in range(col, n):
                    A[i][j] -= factor * A[rank][j]

        rank += 1

    return rank


A = [[3, 2, 5],
     [1, 1, 2],
     [3, 3, 6]]

print(matrix_rank(A))
```

## Output:

<img width="1502" height="985" alt="image" src="https://github.com/user-attachments/assets/eca6da18-3611-499f-8dc5-c37501bec9ca" />


## Result:
Thus the rank for the given matrix is successfully solved by  using a python program.

