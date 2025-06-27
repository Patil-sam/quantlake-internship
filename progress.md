# Quantlake Internship Progress Log

## 📅 Day 1 - Git & GitHub Basics + Python Fundamentals

**Date:** 16th June 2025

---

### ✅ Git Commands Learned and Used:

- `git init`:  
  Initializes a new Git repository in the current directory.

- `git add filename` or `git add .`:  
  Adds file(s) to the staging area so they can be committed.  
  `git add .` adds all changes in the directory.

- `git commit -m "your message"`:  
  Commits the staged changes with a message describing what was done.

- `git remote add origin https://github.com/your-username/repo-name.git`:  
  Links your local repository to a remote GitHub repository.

- `git push -u origin main`:  
  Pushes your committed changes to the main branch on GitHub.

- `git pull origin main`:  
  Pulls the latest changes from the main branch of the remote GitHub repository into your local repository.

---

### 🔧 Repository Setup:

- Created a new repository on GitHub named `quantlake-internship`.
- Initialized a local Git repository using `git init`.
- Connected it to GitHub using `git remote add origin`.
- Pushed the initial commit using `git push -u origin main`.

---

### 📁 Folder Structure Created:
quantlake-internship/
├── training/
│ └── day1_python_basics.ipynb
├── projects/
└── progress.md


---

### 📓 Notebook Added:

- Created a Jupyter Notebook named `day1_python_basics.ipynb`.
- Topics covered in the notebook:
  - Data types: int, float, complex, str, bool
  - Lists, tuples, sets, dictionaries, arrays
  - Conditional statements: if, elif, else
  - Loops: for loop
- Saved the notebook in the `training/` folder.
- Committed and pushed the notebook to GitHub using Git


## 📅 Day 2 -Python structures + functions

- Practiced data structures: `list`, `tuple`, `set`, `dict`
- Explored methods and operations for each structure
- Used list comprehensions and dictionary nesting/lookups
- Wrote custom functions: factorial calculator, prime number checker
- Used built-in modules: `math`, `random`, `datetime`
- Learned and practiced error handling using `try`, `except`, `finally`
- Solved mini problems: FizzBuzz, largest number in a list, reverse string, count vowels


## Day 3: Pandas Introduction

**Notebook:** `day3_pandas_intro`

**Topics Practiced:**
- Created Series and DataFrame from scratch.
- Used `.head()`, `.tail()`, `.shape`, `.columns`, `.index`, `.dtypes` to inspect structure.
- Loaded Titanic dataset using `pd.read_csv()`.
- Explored dataset using `.info()`, `.describe()`, `.isnull().sum()`.
- Identified null values, data types, row and column count.
- Accessed and filtered data using:
  - `df['column']`, `df[['col1', 'col2']]`
  - `df.loc[]`, `df.iloc[]`
- Added new calculated columns like `FamilySize` and `FarePerPerson`.
- Dropped a row using `df.drop()`.
- Practiced built-in methods:
  - `.sort_values()`, `.value_counts()`, `.unique()`
  - `.mean()`, `.sum()`, `.min()`, `.max()`
- Grouped data using `groupby()` to find average fare by class.

**Status:** Completed

## 📅 Day 4: Data Manipulation 1 (`day4_data_manipulation_1`)

### 🔹 Task 1: Indexing and Slicing
- Loaded `Super_Store_Sales_data.csv` using `pd.read_csv()`.
- Practiced:
  - `df.loc[]` for label-based selection.
  - `df.iloc[]` for index-based selection.
  - Selecting full rows, specific columns, and conditional subsets (e.g., `df[df['Sales'] > 500]`).

### 🔹 Task 2: Filtering & Sorting
- Filtered data using boolean logic with `&`, `|`, and conditions on `Sales`, `Ship Date`, `Region`, etc.
- Sorted data by `Sales`, `Profit`, and multiple columns like `['Category', 'Sales']`.

### 🔹 Task 3: Handling Missing Data
- Used `df.isnull().sum()` to find missing values.
- Dropped missing rows using `df.dropna()`.
- Created a DataFrame with `np.nan` values and practiced `fillna()` and inspection techniques.

### 🔹 Task 4: GroupBy Operations
- Used `groupby()` to calculate `mean()` on `Category`.
- Performed aggregations on `Region` and `Sub-Category` with `agg(['sum', 'mean', 'count'])`.
- Used `reset_index()` to clean up grouped results.

### 🔹 Task 5: Merging DataFrames
- Created `orders` and `customers` sample DataFrames.
- Practiced merging using:
  - `pd.merge(..., how='inner')`
  - `pd.merge(..., how='left')`
  - `pd.merge(..., how='outer')`

Completed all data manipulation tasks for Day 4 using the Superstore dataset.


# 📘 Progress Log

## ✅ Task 1: Reshaping DataFrames
- [x] Used `pivot_table()` to get total sales by Region and Category
- [x] Used `pivot_table()` to calculate average profit per Segment
- [x] Used `melt()` to convert wide to long format

## ✅ Task 2: Apply Custom Functions
- [x] Created `Sales_Margin` column using `.apply()` with lambda
- [x] Flagged high discount rows using `.apply()` on `Sales`
- [x] Flagged high sales rows using `.apply()` on `Sales`

## ✅ Task 3: Mapping & Replacing
- [x] Used `.map()` to convert Country to Country Code
- [x] Used `.replace()` to rename "Consumer" to "Retail" in Segment

## ✅ Task 4: Combining DataFrames
- [x] Used `pd.concat()` vertically with `ignore_index=True`
- [x] Used `pd.concat()` horizontally with `axis=1`
- [x] Combined DataFrames with mismatched columns


