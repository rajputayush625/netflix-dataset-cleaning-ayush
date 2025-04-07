# 📊 Task 1 – Data Cleaning and Preprocessing

🔍 Internship Task Overview

As part of the **Data Analyst Internship**, the goal of this task was to clean and preprocess a raw dataset containing Netflix movies and TV shows. The original data had missing values, duplicates, inconsistent formats, and unstandardized fields.


# 📁 Dataset Used

- Source: Netflix Movies and TV Shows dataset from Kaggle
- Original File: `netflix_titles.csv`
- Cleaned File: `netflix_titles_cleaned.csv`

---

# 🧹 Cleaning Steps Performed

1. Removed Duplicate Rows
   - Used `drop_duplicates()` to ensure unique entries.

2. Renamed Columns
   - Converted all column names to lowercase and replaced spaces with underscores.

3. Handled Missing Values
   - `director` and `cast`: Filled with `"Not Available"`
   - `country`: Filled with `"Unknown"`
   - `rating`: Filled with `"Not Rated"`
   - Dropped rows where `date_added` or `duration` was still missing after attempts to clean.

4. Standardized Date Format
   - Converted `date_added` column to `dd-mm-yyyy` format using `pd.to_datetime()`.

5. Cleaned Text Data
   - Stripped extra spaces from text columns like `title`, `type`, `description`, etc.

6. Validated Data Types
   - Ensured all columns had the correct data types after cleaning.


📦 Files Included

- `netflix_titles.csv` – Original dataset
- `netflix_titles_cleaned.csv` – Cleaned dataset
- `task1_cleaning_script.py` – Python script used for cleaning
- `README.md` – This file

📚 Concepts Practiced

- Handling missing data (`fillna`, `dropna`)
- Removing duplicates
- Date formatting and standardization
- Data type validation
- Basic string processing
- Preprocessing for analysis-ready data
