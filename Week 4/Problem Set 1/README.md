# MSoc Pandas Problem Set

## Overview

This problem set is designed to help students learn Pandas progressively. The first three problems focus on Pandas fundamentals using manually created DataFrames. The last three problems use a real-world dataset to perform data analysis.

---

# Problem 1: Create and Explore a DataFrame

## Objective

Learn how to create and inspect a DataFrame.

### Given Data

| Name    | Age | City      |
| ------- | --- | --------- |
| Alice   | 21  | Delhi     |
| Bob     | 19  | Mumbai    |
| Charlie | 22  | Ahmedabad |
| David   | 20  | Pune      |

### Tasks

1. Create the DataFrame.
2. Display the first 2 rows.
3. Display all column names.
4. Find the shape of the DataFrame.
5. Display information about the DataFrame.

---

# Problem 2: Filtering and Selection

## Objective

Learn how to select and filter data.

### Given Data

| Product  | Price | Quantity |
| -------- | ----- | -------- |
| Laptop   | 50000 | 5        |
| Mouse    | 500   | 20       |
| Keyboard | 1500  | 15       |
| Monitor  | 12000 | 7        |

### Tasks

1. Select only the `Product` column.
2. Select the `Product` and `Price` columns.
3. Find products with `Price > 1000`.
4. Find products with `Quantity < 10`.
5. Find products satisfying both conditions.


---

# Problem 3: Data Manipulation

## Objective

Learn how to create new columns and perform calculations.

### Given Data

| Student | Maths | Science |
| ------- | ----- | ------- |
| A       | 85    | 90      |
| B       | 70    | 65      |
| C       | 95    | 88      |
| D       | 60    | 75      |

### Tasks

1. Create a new column called `Total`.
2. Create a new column called `Average`.
3. Find the student with the highest `Total`.
4. Sort the DataFrame by `Average` in descending order.
5. Display students whose `Average` is greater than 80.

---

# Problem 4: Dataset Exploration

## Objective

Learn how to inspect a real-world dataset.

### Dataset

Titanic Dataset
<br>
To download the dataset please run this code.
```py
import kagglehub
import pandas as pd
import os

path = kagglehub.dataset_download("yasserh/titanic-dataset")

print("Path to dataset files:", path)



files_in_directory = os.listdir(path)

csv_file = None
for file in files_in_directory:
    if file.endswith('.csv'):
        csv_file = file
        break

if csv_file:
    full_csv_path = os.path.join(path, csv_file)
    df = pd.read_csv(full_csv_path)
    df.head()
else:
    print(f"No CSV file found in the directory: {path}")
    df = None 

print("Data : " , df)
```

### Tasks

1. Load the dataset using Pandas.
2. Display the first 10 rows.
3. Find the number of rows and columns.
4. Display all column names.
5. Check missing values in each column.
6. Generate summary statistics.


---

# Problem 5: Filtering and Analysis

## Objective

Practice filtering and extracting useful information.

### Dataset

Above Dataset

### Tasks

1. Find all female passengers.
2. Find passengers older than 30 years.
3. Find passengers who survived.
4. Find female passengers who survived.
5. Calculate the average age of passengers.
6. Find the oldest passenger in the dataset.
---

# Problem 6: GroupBy and Insights

## Objective

Perform real-world data analysis using GroupBy.

### Dataset

Titanic Dataset

### Tasks

1. Find the survival rate by gender.
2. Find the average age by passenger class.
3. Count the number of passengers in each class.
4. Find the class with the highest survival rate.
5. Find the average fare paid by each class.
6. Write a short report summarizing your findings.




---

# Expected Learning Outcomes

After completing this problem set, students will be able to:

* Create and manipulate DataFrames.
* Select and filter data efficiently.
* Create new features using existing columns.
* Load and explore datasets.
* Handle missing values.
* Perform statistical analysis.
* Use GroupBy operations.
* Extract meaningful insights from real-world data.

Happy Learning with Pandas! 🚀
