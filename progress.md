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
