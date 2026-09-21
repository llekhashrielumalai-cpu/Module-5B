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

Add code here
import pandas as pd

# Create the first DataFrame
student_data1 = {
    'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],
    'name': ['Danni', 'Raman', 'Alex', 'Soham', 'Kavi'],
    'marks': [200, 210, 190, 222, 199]
}

df1 = pd.DataFrame(student_data1)

# Create the second DataFrame
student_data2 = {
    'student_id': ['S6', 'S7', 'S8', 'S9', 'S10'],
    'name': ['John', 'Sara', 'David', 'Meena', 'Arun'],
    'marks': [188, 205, 215, 195, 220]
}

df2 = pd.DataFrame(student_data2)

# Join the two DataFrames row-wise
new_df = pd.concat([df1, df2], axis=0, ignore_index=True)

# Display the result
print("First DataFrame:")
print(df1)

print("\nSecond DataFrame:")
print(df2)

print("\nCombined DataFrame:")
print(new_df)
## Output
First DataFrame:
  student_id   name  marks
0         S1  Danni    200
1         S2  Raman    210
2         S3   Alex    190
3         S4  Soham    222
4         S5   Kavi    199

Second DataFrame:
  student_id   name  marks
0         S6   John    188
1         S7   Sara    205
2         S8  David    215
3         S9  Meena    195
4        S10   Arun    220

Combined DataFrame:
  student_id   name  marks
0         S1  Danni    200
1         S2  Raman    210
2         S3   Alex    190
3         S4  Soham    222
4         S5   Kavi    199
5         S6   John    188
6         S7   Sara    205
7         S8  David    215
8         S9  Meena    195
9        S10   Arun    220
## Result
Thus, the Pandas program was successfully executed to join two DataFrames along rows using pd.concat() with axis=0.
