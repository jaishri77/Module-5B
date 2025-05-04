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

exam_data = {
    'name': ['Alice', 'Bob', 'Charlie', 'David'],
    'score': [85, 92, 78, 88],
    'attempts': [1, 2, 1, 3],
    'qualify': ['Yes', 'Yes', 'No', 'Yes']
}

labels = ['A', 'B', 'C', 'D']
df = pd.DataFrame(exam_data, index=labels)
print(df)
```

## Output
```
      name  score  attempts qualify
A    Alice     85         1     Yes
B      Bob     92         2     Yes
C  Charlie     78         1      No
D    David     88         3     Yes
```
## Result
The program creates and displays a DataFrame from a given dictionary, using custom index labels for the rows.
