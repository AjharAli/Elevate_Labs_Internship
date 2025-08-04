# 📺 Netflix Data Cleaning

This project contains data cleaning steps performed on the Netflix dataset. The goal is to preprocess and clean the data for accurate and efficient analysis.

-------  I cleaned this data ussing both MS Excel and Python(Pandas).

Dataset Link- https://www.kaggle.com/datasets/shivamb/netflix-shows/data

## 🗂 Dataset Overview

The dataset includes information about Netflix titles such as:
- Title
- Type (Movie/TV Show)
- Director, Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Description
- Categories/Genres

---

## 🧹 Data Cleaning Steps

### 1. **Importing the Dataset**
- Loaded the dataset using `pandas.read_csv()`

### 2. **Initial Data Inspection**
- Used `.head()`, `.info()`, and `.describe()` to get an overview
- Checked for null values using `.isnull().sum()`

### 3. **Handling Missing Values**
- Filled missing `country`, `cast`, and `director` values with `"Unknown"`
- Converted `date_added` to datetime format using `pd.to_datetime()`
- Replaced empty strings with NaN where appropriate

### 4. **Removing Duplicates**
- Checked for duplicate rows using `.duplicated()`
- Removed duplicates using `.drop_duplicates()`

### 5. **Standardizing Columns**
- Trimmed extra spaces in string columns using `.str.strip()`
- Converted all text columns to lowercase for consistency

### 6. **Converting Data Types**
- Converted `release_year` to `int`
- Converted `date_added` to `datetime64`
- Cleaned and standardized `duration` column (e.g., extracted numeric value and unit)

### 7. **Handling Inconsistent Entries**
- Standardized `rating` values (e.g., unified formats like `"TV-MA"`, `"PG-13"`)
- Cleaned `duration` field to separate duration type (minutes/seasons)

---

## ✅ Final Result

After cleaning:
- All null values are handled
- Text fields are consistent and standardized
- Date and numerical formats are correctly parsed
- The dataset is ready for visualization or model-building

---

## 📂 Files
- `netflix_titles.csv` – Original dataset
- `Task-1.ipynb` – Jupyter notebook with step-by-step code

---

## 📌 Tools Used
- MS Excel
- Python
- Pandas

---

## ✍️ Author
Ajhar Ajhar Ali  
*Intern | Data Enthusiast*

---

## 📬 Contact
- GitHub: (https://github.com/AjharAli/))
- Email: ajharalimbdgmail.com
