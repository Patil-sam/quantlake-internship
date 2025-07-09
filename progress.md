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




## 📊 Data Visualization Progress — Iris Dataset

### ✅ Task 1: Matplotlib Basics
- Imported `matplotlib.pyplot as plt`
- Created:
  - Line plot of Sepal Length across sample IDs
  - Scatter plot of Sepal Length vs Petal Length
- Saved figures with `plt.savefig()` using `dpi=300`

### ✅ Task 2: Plot Customization
- Added:
  - Titles, X/Y-axis labels, legends
  - Gridlines for better readability
  - Axis limits and custom figure sizes
- Improved overall layout and clarity

### ✅ Task 3: Seaborn Introduction
- Imported `seaborn as sns`
- Created:
  - Boxplot of Sepal Length by Species (outlier detection)
  - Heatmap of correlation between all features
  - Histogram of Petal Length with KDE
- Used Seaborn styles for visual enhancement

### ✅ Task 4: Sample Visualization Project
- Chose Iris dataset for a mini project
- Created multiple charts:
  - Histogram: Petal Length distribution
  - Line Plot: Sepal Length across sample IDs
  - Boxplot: Petal Width by Species
- Analyzed distributions and trends across species

### ✅ Task 5: Produce Publish-Quality Figures
- Refined the boxplot to publication standards:
  - Used `dpi=300`, modern color palette (`Set2`)
  - Applied `sns.set_theme()` for clean visuals
  - Adjusted font sizes, layout, and removed spines using `sns.despine()`
  - Exported as `iris_boxplot_published.png`

---

✅ **Status**: All 5 tasks completed  
📁 **Dataset used**: Iris Dataset (`iris.csv`)  
🖼️ **Figures saved in**: `*.png` files (300 DPI, ready for presentation/report)



# 📊 Day 7 SQL Intro – Progress Report

## ✅ Database Used:
**SQLite 3**  
**Database file**: `chinook.db`  
**Location**: E:\QuantLake

## 📁 Files Submitted:
- `day7_sql_intro.sql` – Contains all SQL queries for Tasks 1 to 5
- `day7_sql_output.txt` – Contains query results (captured from SQLite prompt)

## 🧠 Tasks Completed:

### 🔹 Task 1: Understand Tables and Fields
- Listed all tables using `.tables`
- Inspected table structures using `PRAGMA table_info(...)` for:
  - albums
  - artists
  - customers
  - employees
  - genres
  - invoice_items
  - invoices
  - tracks

### 🔹 Task 2: SELECT Queries
- Viewed full customer table:  
  `SELECT * FROM customers;`
- Selected specific employee columns:  
  `SELECT FirstName, LastName FROM employees;`

### 🔹 Task 3: Filtering with WHERE
- Invoices with Total > 10  
  `SELECT * FROM invoices WHERE Total > 10;`
- Customers from USA  
  `SELECT * FROM customers WHERE Country = 'USA';`
- Tracks with 'Rock' in Composer  
  `SELECT * FROM tracks WHERE Composer LIKE '%Rock%';`

### 🔹 Task 4: Sorting and Limiting
- Top 5 invoices by amount  
  `SELECT * FROM invoices ORDER BY Total DESC LIMIT 5;`
- First 3 tracks alphabetically  
  `SELECT * FROM tracks ORDER BY Name ASC LIMIT 3;`

### 🔹 Task 5: Basic Aggregations
- Total customers:  
  `SELECT COUNT(*) FROM customers;`
- Average invoice amount:  
  `SELECT AVG(Total) FROM invoices;`
- Sales by country:  
  `SELECT BillingCountry, SUM(Total) FROM invoices GROUP BY BillingCountry ORDER BY SUM(Total) DESC;`

## ⭐ 5 Interesting Queries:
1. `SELECT FirstName, LastName FROM employees;`
2. `SELECT * FROM customers WHERE Country = 'USA';`
3. `SELECT * FROM invoices WHERE Total > 10;`
4. `SELECT * FROM tracks WHERE Composer LIKE '%Rock%';`
5. `SELECT BillingCountry, SUM(Total) FROM invoices GROUP BY BillingCountry ORDER BY SUM(Total) DESC;`

## 📸 Screenshots:
SQL outputs are saved in `day7_sql_output.txt`



