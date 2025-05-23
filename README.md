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

