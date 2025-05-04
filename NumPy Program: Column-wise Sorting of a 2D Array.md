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
```
import numpy as np
arr = np.array([[9, 8, 7],
                [6, 5, 4],
                [3, 2, 1]])
sorted_arr = np.sort(arr, axis=0)
print("Original array:")
print(arr)
print("Column-wise sorted array:")
print(sorted_arr)
```

## Output
```
Original array:
[[9 8 7]
 [6 5 4]
 [3 2 1]]
Column-wise sorted array:
[[3 2 1]
 [6 5 4]
 [9 8 7]]
```
## Result
The program sorts each column of the given 2D array in ascending order.
