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
    'name': ['Alice', 'Bob'],
    'age': [20, 22],
    'score': [85, 92]
}

student_data2 = {
    'name': ['Charlie', 'David'],
    'age': [21, 23],
    'score': [78, 88]
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

combined_df = pd.concat([df1, df2], axis=0, ignore_index=True)
print(combined_df)
```

## Output
```
      name  age  score
0    Alice   20     85
1      Bob   22     92
2  Charlie   21     78
3    David   23     88
```

## Result
The program concatenates two DataFrames row-wise using pd.concat() and displays the combined DataFrame.
