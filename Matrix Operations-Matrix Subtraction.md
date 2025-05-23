# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
    rows = int(input(f"Enter number of rows for {name}: "))
    cols = int(input(f"Enter number of columns for {name}: "))
    
    print(f"Enter elements of {name} row-wise ({rows} x {cols}):")
    matrix = []
    for i in range(rows):
        row = list(map(int, input(f"{name} - Row {i + 1}: ").split()))
        if len(row) != cols:
            print("❌ Invalid number of columns. Please restart.")
            exit()
        matrix.append(row)
    return matrix, rows, cols

def subtract_matrices(matrix1, matrix2):
    return [
        [matrix1[i][j] - matrix2[i][j] for j in range(len(matrix1[0]))]
        for i in range(len(matrix1))
    ]
def print_matrix(matrix, title="Result"):
    print(f"\n{title}:")
    for row in matrix:
        print(' '.join(f"{val:4}" for val in row))
matrix1, rows1, cols1 = read_matrix("Matrix A")
matrix2, rows2, cols2 = read_matrix("Matrix B")
if rows1 != rows2 or cols1 != cols2:
    print("❌ Matrices must have the same dimensions for subtraction.")
else:
    result = subtract_matrices(matrix1, matrix2)
    print_matrix(matrix1, "Matrix A")
    print_matrix(matrix2, "Matrix B")
    print_matrix(result, "Matrix A - Matrix B")
```
## OUTPUT:
![444430186-a1b6b15a-7275-4bf5-bef2-cd4c312c2e9e](https://github.com/user-attachments/assets/79a04e05-b13e-4cac-8d0a-fd95c054d36d)

## RESULT:
Thus the program has been executed successfully.
