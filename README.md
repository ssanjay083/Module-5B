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
arr = np.array([[12, 5, 7], [4, 8, 6], [9, 3, 1]])
sorted_arr = np.sort(arr, axis=0)
print("Original Array:\n", arr) print("Column-wise Sorted Array:\n", sorted_arr)
```

## Output
![439804946-ce397dbd-45bd-4611-9781-e1ee728414be](https://github.com/user-attachments/assets/6df98a7b-360a-4ed2-a176-7f86f9059e16)

## Result

Thus the program has been successfully executed.

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

```
import numpy as np
x = np.array([5, 8, 2, 9, 6])
indices = np.where(x >= y)
y = np.array([3, 8, 4, 7, 6])
print("Array x:", x) print("Array y:", y) print("Indices where x >= y:", indices[0])
```
## Output
![439805383-e4b4a900-ec3f-49eb-b501-0dd4f70ccd96](https://github.com/user-attachments/assets/bd51e82a-79df-464f-aee4-eb97ac09eb09)

## Result
Thus the program has been successfully executed.

# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])

new_col = np.array([10, 11, 12])

arr_modified = np.delete(arr, 1, axis=1)

arr_updated = np.insert(arr_modified, 1, new_col, axis=1)

print("Updated Array:\n", arr_updated)
```
## Output
![439805763-4c131933-f724-4451-8506-f623b110c87c](https://github.com/user-attachments/assets/13ff986e-fb8e-452b-973e-b15a847b7760)

## Result
Thus the program has been successfully executed.

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---


## 💻 Program
```
import pandas as pd
import numpy as np

exam_data = {
    'name': ['Anu', 'Bala', 'Chitra', 'David', 'Eva'],
    'score': [85, 92, 76, 88, 90],
    'attempts': [1, 2, 1, 3, 2],
    'qualify': ['yes', 'yes', 'no', 'yes', 'yes']
}

labels = ['a', 'b', 'c', 'd', 'e']

df = pd.DataFrame(exam_data, index=labels)

# Display output
print("Result:\n", df)
```

## Output
![439806517-d197e499-3f0c-4222-be33-8e3d5404aecd](https://github.com/user-attachments/assets/7410892b-8275-494a-a2e1-0f7dfb08395e)
## Result
Thus the program has been successfully executed

# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---


## 💻 Program
```
import pandas as pd

student_data1 = {
    'name': ['geri', 'sharun'],
    'age': [20, 22],
    'score': [85, 92]
}

student_data2 = {
    'name': ['muthu', 'vicky'],
    'age': [23, 21],
    'score': [76, 88]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

df_combined = pd.concat([df1, df2], axis=0, ignore_index=True)

print("Result:\n", df_combined)
```

## Output
![439813711-6202671b-db26-427f-9fc5-59caf7b83e4d](https://github.com/user-attachments/assets/a49b6648-00a5-4f76-a2c8-fbbdce732cb6)
## Result
Thus the program has been successfully executed
