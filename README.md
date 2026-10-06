# Pandas Data Analysis Assessments

A comprehensive collection of data analysis and cleaning exercises using **Python** and **Pandas**. This repository contains four real-world business scenarios covering e-commerce, healthcare, banking, and energy sectors.

---

## Table of Contents

- Overview
- [Projects](#projects)
  - [Exercise 1: E-Commerce Customer Analysis](#exercise-1-e-commerce-customer-analysis)
  - [Exercise 2: Hospital Patient Data Cleaning](#exercise-2-hospital-patient-data-cleaning)
  - [Exercise 3: Banking Customer Transaction Analysis](#exercise-3-banking-customer-transaction-analysis)
  - [Exercise 4: Energy Consumption Analysis](#exercise-4-energy-consumption-analysis)
- [Technologies Used](#technologies-used)
- [Key Skills Demonstrated](#key-skills-demonstrated)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Overview

This repository showcases practical data analysis skills applied to four different industry datasets. Each exercise follows a structured workflow:

1. **Data Loading & Inspection** — Understanding the dataset structure
2. **Data Cleaning** — Handling missing values, duplicates, and inconsistencies
3. **Data Transformation** — Creating new features and categories
4. **Data Analysis** — Extracting insights and answering business questions
5. **Business Recommendations** — Translating data into actionable strategies

---

## Projects

### Exercise 1: E-Commerce Customer Analysis
**Domain:** E-Commerce / Retail

**Dataset:** `customer_sales.csv` (5,000 records, 7 columns)

**Key Tasks:**
- Loaded and inspected customer sales data
- Analyzed customer distribution across cities
- Examined product category performance
- Classified customers as "High Value" (Sales ≥ ₦100,000) vs "Standard"
- Identified 2,983 high-value customers

**Key Insights:**
- Enugu had the highest customer count (364)
- Home Appliances was the most frequent product category
- 3,099 completed orders out of 5,000 total

---

### Exercise 2: Hospital Patient Data Cleaning
**Domain:** Healthcare

**Dataset:** `hospital_patient_data_cleaning_practice.csv` (3,000 records, 8 columns)

**Key Tasks:**
- Identified data quality issues (missing values, text in numeric columns)
- Cleaned inconsistent city names (e.g., "lagos" → "Lagos")
- Converted text numbers to numeric (e.g., "six" → 6)
- Removed test/dummy records (Patient IDs 9000+)
- Classified patients as "Frequent" (≥5 visits) vs "Occasional"
- Reduced dataset from 3,000 to 2,909 clean records

**Key Insights:**
- 1,962 Frequent Patients (average 8.5 visits)
- 947 Occasional Patients (average 2.5 visits)
- Frequent patients represent a strong base of loyal, returning patients

---

### Exercise 3: Banking Customer Transaction Analysis
**Domain:** Banking / Financial Services

**Dataset:** `Banking_Customer_Transation.csv` (3,000 records, 6 columns)

**Key Tasks:**
- Investigated transaction amounts for errors
- Handled missing values and unexpected text (e.g., "Error", "##VALUE!")
- Removed invalid records (negative, zero, and extreme outlier amounts)
- Classified transactions as "Large" (≥ ₦100,000) vs "Regular"
- Reduced dataset from 3,000 to 2,795 clean records

**Key Insights:**
- Lagos had the highest transaction volume (681)
- Benin City had the highest average transaction amount (₦52,154)
- 276 large transactions identified
- Transfer was the most frequent transaction type

---

### Exercise 4: Energy Consumption Analysis
**Domain:** Energy / Utilities

**Dataset:** `Energy_Consumption.csv` (3,012 records, 6 columns)

**Key Tasks:**
- Inspected data types and summary statistics
- Cleaned missing city and consumption values
- Removed duplicates and invalid (negative/zero) consumption records
- Classified consumption as "High" (≥ 500 kWh) vs "Normal"
- Reduced dataset from 3,012 to 2,748 clean records

**Key Insights:**
- Industrial customers consumed the most energy (6,490 kWh avg)
- Residential customers were the largest group (1,417)
- Grid Electricity was the primary energy source
- 1,261 high-consumption customers identified

---

## Technologies Used

| Technology | Purpose |
|------------|---------|
| **Python 3.13** | Programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical and vectorized operations |
| **Jupyter Notebook** | Interactive development environment |

---

## Key Skills Demonstrated

### Data Loading & Inspection
- `pd.read_csv()` — Loading CSV files
- `.head()`, `.shape`, `.info()`, `.describe()` — Data inspection
- `.dtypes` — Checking data types

### Data Cleaning
- `.isnull().sum()` — Identifying missing values
- `.dropna()` — Removing missing values
- `.fillna()` — Filling missing values
- `.drop_duplicates()` — Removing duplicates
- `pd.to_numeric(errors='coerce')` — Converting text to numeric
- `.replace()` — Replacing inconsistent values
- `.str.title()` — Standardizing text casing

### Data Transformation
- `np.where()` — Conditional column creation
- `.astype()` — Type conversion
- `.apply()` — Applying functions to columns

### Data Analysis
- `.value_counts()` — Frequency analysis
- `.mean()`, `.median()`, `.std()` — Statistical measures
- `.groupby()` — Grouping data
- `.agg()` — Aggregating multiple statistics
- `.sort_values()` — Sorting results

## Sample Output

<img width="1125" height="637" alt="pd1" src="https://github.com/user-attachments/assets/6a998ce7-9320-4066-844e-c4cb9849718c" />

<img width="1104" height="542" alt="pd2" src="https://github.com/user-attachments/assets/7fe7be1f-eec7-4735-a600-2a7a001a5b0f" />

<img width="1139" height="538" alt="pd3" src="https://github.com/user-attachments/assets/29b7879e-50f6-4719-89c3-2c2c2f5037e6" />

<img width="1148" height="554" alt="pd4" src="https://github.com/user-attachments/assets/60480870-b928-4170-b28f-0e9afcfab439" />

<img width="1124" height="547" alt="pd5" src="https://github.com/user-attachments/assets/7d92eb55-7727-4b2d-a512-5bc4e723f968" />

<img width="1099" height="549" alt="pd6" src="https://github.com/user-attachments/assets/ab8c9953-579f-4ba1-9891-0c2f02fbbdcf" />

<img width="1130" height="514" alt="pd7" src="https://github.com/user-attachments/assets/79580f0f-889a-4bb4-b4a0-d6b8c8ed54e8" />

<img width="1096" height="539" alt="pd8" src="https://github.com/user-attachments/assets/1cc136c2-ea66-4652-95b9-b3c05b61bfa4" />

---

## NumPy Concepts Covered

Concept Functions / Methods Used
Data Loading pd.read_csv(), pd.DataFrame()
Data Inspection .head(), .shape, .info(), .describe()
Missing Values .isnull(), .sum(), .dropna(), .fillna()
Data Type Conversion pd.to_numeric(), .astype()
String Operations .str.title(), .str.contains(), .replace(), .unique()
Duplicates .duplicated(), .drop_duplicates()
Filtering Boolean masks, .between(), ~ operator
Grouping .groupby(), .agg(), .value_counts(), .mode()
Conditional Columns np.where()
Sorting .sort_values()
Reshaping .reset_index(), .to_string()
Formatting f-strings, .round(), .apply()


## Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Emmanouhl/pandas-data-analysis-assessments.git
cd pandas-data-analysis-assessments

---

pandas-data-analysis-assessments/
│
├── README.md
│
├── Exercise_1_Ecommerce_Customer_Analysis.ipynb
├── Exercise_2_Hospital_Patient_Data_Cleaning.ipynb
├── Exercise_3_Banking_Transaction_Analysis.ipynb
├── Exercise_4_Energy_Consumption_Analysis.ipynb
│
├── data/
│   ├── customer_sales.csv
│   ├── hospital_patient_data_cleaning_practice.csv
│   ├── Banking_Customer_Transation.csv
│   └── Energy_Consumption.csv
│
└── requirements.txt

Author

Mustapha Emmanuel Oladeji

📧 Email: [mustaphaemmanuelola@gmail.com]
🔗 LinkedIn: [https://linkedin.com/in/mustaphaemmanouelola]
🐙 GitHub: [https://github.com/Emmanouhl]

---

Acknowledgments

This project was completed as part of the Python Study Group – Lesson 16: Pandas Data Analysis hands-on practice.

---

License

This project is open for educational and portfolio purposes.

---

Built with Pandas – Turning raw data into business intelligence.

Happy Analyzing!
