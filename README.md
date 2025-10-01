# Experiment 8 - 2D Array in C++

---

## Aim
- To understand and implement two-dimensional arrays in C++, exploring their structure, operations, and applications in matrix manipulation.

---

## Tools Used
- Visual Studio Code
- MinGW-w64 with g++ Compiler

---

## Theory
A **2D array** is a grid-like data structure where elements are stored in rows and columns. It is essentially an "array of arrays," allowing for the natural representation of matrices and other tabular data. Key characteristics include:
- Fixed dimensions (rows and columns) defined at compile time.
- Accessed using two indices: `array[row][column]`.
- Useful for matrix operations, image processing, and game boards.

### Common Operations
- **Input/Output:** Using nested loops to read and display matrix elements.
- **Transpose:** Flipping the matrix over its diagonal by swapping rows and columns (`new_matrix[j][i] = old_matrix[i][j]`).
- **Addition:** Performing an element-wise sum of two matrices of the same dimensions.
- **Multiplication:** Calculating the dot product of rows and columns from two matrices.

---

## Algorithm / Logic

### Program 1: Matrix Transpose
1.  **Start**
2.  Declare an original matrix `a[rows][cols]` and a transpose matrix `b[cols][rows]`.
3.  Prompt the user to enter the elements of the original matrix.
4.  Use a nested loop to iterate through `i` (rows) and `j` (columns) of the original matrix.
5.  Inside the loop, assign `b[j][i] = a[i][j]`.
6.  After the loops complete, print the transposed matrix `b`.
7.  **End**

### Program 2: Matrix Addition
1.  **Start**
2.  Declare three matrices of the same dimensions: `a`, `b`, and `sum`.
3.  Prompt the user to enter the elements for matrices `a` and `b`.
4.  Use a nested loop to iterate through `i` (rows) and `j` (columns).
5.  Inside the loop, add the corresponding elements: `sum[i][j] = a[i][j] + b[i][j]`.
6.  Print the resulting `sum` matrix.
7.  **End**

### Program 3: Matrix Multiplication
1.  **Start**
2.  Declare matrices `A[r1][c1]`, `B[r2][c2]`, and the result `C[r1][c2]`. Initialize `C` with zeros.
3.  Check if `c1 == r2`. If not, multiplication is not possible.
4.  Use three nested loops (for `i`, `j`, and `k`).
5.  Multiply and accumulate the results: `C[i][j] += A[i][k] * B[k][j]`.
6.  Print the resulting matrix `C`.
7.  **End**

### Program 4: Diagonal Sum
1.  **Start**
2.  Declare a square matrix `a[n][n]` and initialize a variable `sum = 0`.
3.  Prompt the user to enter the matrix elements.
4.  Loop from `i = 0` to `n-1`.
5.  Inside the loop, add the main diagonal element `a[i][i]` to `sum`.
6.  (Optional) Add the anti-diagonal element `a[i][n-1-i]` to the sum if needed.
7.  Print the final `sum`.
8.  **End**

---

## Conclusion
Two-dimensional arrays are essential for representing structured data in C++. Mastering operations like transpose, addition, and multiplication builds a strong foundation for solving complex matrix-based problems. Through careful indexing and the use of nested loops, programmers can manipulate 2D arrays efficiently. These skills are crucial for applications in scientific computing, graphics, and data analysis.
