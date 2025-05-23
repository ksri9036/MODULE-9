# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:
```
    def __init__(self, start, end):
        self.start = start
        self.end = end
        self.even_numbers = self._generate_even_numbers()
    def _generate_even_numbers(self):
        return [num for num in range(self.start, self.end + 1) if num % 2 == 0]
    def get_even_numbers(self):
        return self.even_numbers
generator = EvenNumberGenerator(200, 300)
print(generator.get_even_numbers())
```
## OUTPUT:
![444427940-8286475d-e5c1-44a6-bc22-f6cfb26738da](https://github.com/user-attachments/assets/386e8e80-d4fc-49a8-838e-9f55a90ce7f0)

## RESULT:
Thus the program has been executed successfully.

# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:
```
    def __init__(self, matrix):
        self.matrix = matrix
        self.transposed = self._transpose()
    def _transpose(self):
        return [[self.matrix[row][col] for row in range(len(self.matrix))] 
                for col in range(len(self.matrix[0]))]
    def get_transposed(self):
        return self.transposed
matrix = [
    [1, 2, 3],
    [4, 5, 6]
]

transpose_obj = MatrixTranspose(matrix)
print("Original Matrix:")
for row in matrix:
    print(row)
print("\nTransposed Matrix:")
for row in transpose_obj.get_transposed():
    print(row)
```
## OUTPUT:
![444428742-f3a17be1-f152-4eb9-ba8f-07c1155a42ac](https://github.com/user-attachments/assets/ae6de118-2ae9-418e-93b5-e1243c3e6b01)

## RESULT:
Thus the program has been executed successfully.

# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
    rows = int(input("Enter number of rows: "))
    cols = int(input("Enter number of columns: "))
    print(f"Enter elements row-wise ({rows} x {cols}):")
    matrix = []
    for i in range(rows):
        row = list(map(int, input(f"Row {i + 1}: ").split()))
        if len(row) != cols:
            print("❌ Invalid number of columns. Please restart.")
            exit()
        matrix.append(row)
    return matrix
def print_diagonals(matrix):
    rows = len(matrix)
    cols = len(matrix[0])
    print("\nDiagonal Elements:")
    for i in range(rows):
        for j in range(cols):
            if i == j:
                print(f"{matrix[i][j]:>4}", end=' ')
            else:
                print("    ", end=' ')
        print()
matrix = read_matrix()
print("\nOriginal Matrix:")
for row in matrix:
    print(row)
print_diagonals(matrix)
```
### Output:
![444429540-2c336df4-d635-4b9b-8092-6cabcc51624a](https://github.com/user-attachments/assets/6a339bc4-13bb-4230-9caa-370341fde92c)

## Result
Thus the program has been executed successfully.

