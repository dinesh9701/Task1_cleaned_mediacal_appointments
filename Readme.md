# Task 1 – Data Cleaning and Preprocessing

## 📁 Dataset: Medical Appointment No Shows (Kaggle)

Link: [https://www.kaggle.com/datasets/joniarroba/noshowappointments](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

---

## 🧹 Objective:
To clean and pre-process the dataset by removing errors, fixing inconsistent formatting, and preparing it for analysis or modeling.

---

## 🔧 Tools Used:
- Python
- Pandas (Jupyter Notebook)
- Excel (for verification)

---

## ✅ Cleaning Steps Performed:

### 1. Handled Missing Data
- Checked for missing values using `.isnull().sum()`
- Result: **No missing values** found across all columns

### 2. Removed Duplicates
- Used `.duplicated().sum()` to identify duplicates
- Result: **No duplicate rows**

### 3. Fixed Invalid `age` Entries
- Identified invalid entries: `age = -1` and `age = 0`
- Removed rows where `age <= 0`
- Ensured only patients with valid age values (≥ 1)

### 4. Cleaned `handcap` Column
- Original values ranged from 0 to 4
- Simplified to binary: **0 (not handicapped)** and **1 (handicapped)**

### 5. Standardized Column Names
- Converted all column names to lowercase
- Replaced spaces with underscores for consistency

### 6. Converted Date Columns
- Converted `scheduledday` and `appointmentday` to `datetime` format
- Extracted only the **date part** (removed time)

### 7. Verified Categorical Columns
- Checked and preserved consistent values:
  - `gender`: 'F', 'M'
  - `no-show`: 'Yes', 'No'

### 8. Exported Cleaned Dataset
- Saved as `cleaned_medical_appointments.csv` for submission
- Also converted to `.xlsx` for Excel compatibility

---

## 🧾 Final Output:
- **Cleaned CSV File:** `cleaned_medical_appointments.csv`
- **Formatted Excel File:** `cleaned_medical_appointments.xlsx`
- **Summary Document:** `Data_Cleaning_Summary_Medical_Appointment_No_Shows.docx`

---

## 🧠 Learning Outcome:
- Improved understanding of real-world data quality issues
- Practiced using Pandas for missing values, type conversion, and standardization
- Prepared a structured dataset ready for analysis or modeling

---

## 🔗 Submission Link:
[Paste your GitHub repository URL here]
