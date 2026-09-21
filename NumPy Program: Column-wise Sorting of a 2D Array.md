# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
Add code here
import numpy as np

# Create a 2D array
arr = np.array([[9, 4, 7],
                [3, 8, 2],
                [6, 1, 5]])

# Sort each column in ascending order
sorted_arr = np.sort(arr, axis=0)

# Display the arrays
print("Original Array:")
print(arr)

print("\nColumn-wise Sorted Array:")
print(sorted_arr)
## Output
Original Array:
[[9 4 7]
 [3 8 2]
 [6 1 5]]

Column-wise Sorted Array:
[[3 1 2]
 [6 4 5]
 [9 8 7]]
## Result
Thus, the NumPy program was successfully executed to sort the elements of each column of a 2D array in ascending order using np.sort() with axis=0.
