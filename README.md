# pakistan-eda-project
# 🇵🇰 Pakistan Census Exploratory Data Analysis (EDA)

## 📊 Project Overview
This project performs Exploratory Data Analysis (EDA) on Pakistan census-based demographic and administrative data. The goal is to understand population distribution, urbanization trends, gender composition, and regional differences across Pakistan using real-world structured data.

The analysis is done using Python in a Jupyter Notebook with pandas-based data exploration techniques.

---

## 📁 Dataset Information
- **Source:** Kaggle (Pakistan Census Dataset)
- **Type:** Demographic / Population / Administrative Data
- **Rows:** 10,000+ (approx.)
- **Columns:** 17
- **Geographic Coverage:** Pakistan (Province, District, Tehsil levels)
- **Time Basis:** Derived from Pakistan Census 2017

---

## 📌 Key Features (Columns)
- adm_lvl_1 → Province  
- adm_lvl_2 → Division  
- adm_lvl_3 → District  
- adm_lvl_4 → Tehsil/Sub-division  
- area_name → Name of area  
- area_type → Total / Urban / Rural  
- total_pop → Total population  
- total_male → Male population  
- total_female → Female population  
- total_trans → Transgender population  
- sex_ratio → Male-to-female ratio  
- pop_density → Population per sq km  
- pct_urban → Urban population percentage  
- avg_hh_size → Average household size  
- total_pop_98 → Population in 1998  
- avg_annual_growth → Annual growth rate  

---

## 🧪 Project Workflow

### 1. Data Loading
- Loaded dataset using pandas
- Inspected structure using `.shape`, `.info()`, `.head()`

### 2. Data Cleaning
- Identified missing values using `.isnull().sum()`
- Handled hierarchical structure (province → tehsil levels)
- Separated TOTAL, URBAN, and RURAL records for correct analysis

### 3. Exploratory Data Analysis
- Province-wise population comparison
- Urban vs rural population distribution
- Gender distribution analysis
- Population density analysis
- Growth rate comparisons
- Identification of top populated regions

### 4. Data Quality Checks
- Missing values analysis
- Outlier detection using IQR method
- Structural hierarchy handling
- Detection of inconsistent aggregation levels

---

## 📊 Key Insights
- Punjab has the highest population among all provinces.
- Rural population is higher than urban population in most regions.
- Significant variation exists in population density across districts.
- Urban regions show higher population concentration.
- Growth rates vary across provinces, indicating uneven development.

---

## ⚠️ Data Quality Issues
- Missing values exist in area and density-related columns due to hierarchical structure.
- Some variables are only available at aggregated levels (TOTAL rows).
- Overlapping records exist due to multiple administrative levels.
- Outliers are present but mostly reflect real-world population differences.

---

## 🔮 Future Work (Week 2)
- Handle missing values using appropriate imputation methods
- Improve outlier validation and filtering
- Perform advanced statistical analysis
- Create visualizations (matplotlib/seaborn)
- Build interactive dashboards

---

## 🛠 Tools Used
- Python
- Pandas
- NumPy
- Jupyter Notebook
- Git & GitHub

---

## 👤 Author
Student EDA Internship Project (Pakistan Dataset Analysis)

---

## 📌 Note
This project is part of an internship assignment focusing on real world data exploration, data quality assessment, and basic statistical analysis.
