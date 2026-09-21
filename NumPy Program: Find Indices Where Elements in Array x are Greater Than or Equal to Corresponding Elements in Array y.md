# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program

Add code here
import numpy as np

# Define two arrays
x = np.array([10, 25, 15, 30, 20])
y = np.array([5, 25, 20, 15, 20])

# Find indices where x >= y
indices = np.where(x >= y)

# Display the arrays
print("Array x:", x)
print("Array y:", y)

# Display the indices
print("Indices where x >= y:", indices[0])
## Output
Array x: [10 25 15 30 20]
Array y: [ 5 25 20 15 20]
Indices where x >= y: [0 1 3 4]
## Result
Thus, the NumPy program was successfully executed to find the indices where the elements of array x are greater than or equal to the corresponding elements of array y.
