# Data Cleaning with Pandas 

This repository contains a Jupyter Notebook demonstrating practical data cleaning techniques using Python and the pandas library. The dataset used in this project is the Netflix titles dataset.

##  Contents
- `cleaning.ipynb` – Jupyter Notebook showcasing:
  - Handling missing values
  - Removing duplicates
  - Standardizing column names
  - Converting data types
  - Filtering and sorting data

##  Dataset
The dataset used is `netflix_titles.csv`, containing information about TV shows and movies available on Netflix.
---

## 🔍 What We Do in This Notebook

This notebook walks through a realistic end-to-end data cleaning pipeline using pandas:

1. **Load the Dataset**
   - Read the raw `.csv` file using `pd.read_csv()`.

2. **Initial Exploration**
   - Display the first few rows
   - Check column names and datatypes
   - Use `info()` and `describe()` for a quick summary

3. **Handle Missing Values**
   - Identify columns with missing data
   - Drop rows with critical missing fields (like `title`)
   - Fill or impute less critical fields (like `rating` or `date_added`)

4. **Remove Duplicates**
   - Use `duplicated()` to find repeated entries
   - Drop exact duplicates to maintain dataset integrity

5. **Clean Column Names**
   - Normalize column names by:
     - Lowercasing all names
     - Replacing spaces with underscores
     - Removing special characters (if necessary)

6. **Convert Data Types**
   - Convert `date_added` to datetime
   - Ensure numeric fields (like `release_year`) are integers

7. **Filtering and Sorting**
   - Filter by year, country, or type (e.g., only “Movies”)
   - Sort by `release_year` or `date_added` for better readability

8. **Export the Cleaned Data (optional)**
   - Save the cleaned DataFrame back to a CSV using `to_csv()`

This structured approach ensures the data is analysis-ready and avoids issues during downstream tasks like visualization or machine learning.

---

##  Getting Started

### Requirements
- Python 3.x
- pandas
- Jupyter Notebook or VSCode with Jupyter extension


