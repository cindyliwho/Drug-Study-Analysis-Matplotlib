# Pymaceuticals Drug Study Analysis (Data Analysis & Visualization)

## Overview
This project analyzes data from a **pharmaceutical study** that evaluated the effectiveness of multiple drug regimens on tumor volume in mice. Using Python-based data analysis and visualization, the project compares treatment performance, identifies trends over time, and applies basic statistical methods to draw conclusions about drug efficacy.

The analysis focuses on **Capomulin**, a drug of interest, and compares it against other treatment regimens.

---

## Dataset
The project uses two datasets that are merged for analysis:

- **Mouse_metadata.csv**
  - Mouse ID
  - Drug regimen
  - Sex
  - Age (months)
  - Weight (g)

- **Study_results.csv**
  - Tumor volume (mm³)
  - Timepoints
  - Metastatic sites

---

## Technologies Used
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **SciPy**
- **Jupyter Notebook**

Key libraries:
- `pandas`
- `numpy`
- `matplotlib.pyplot`
- `scipy.stats`

---
## Analysis Workflow

### 1) Data Preparation
- Merge mouse metadata and study results on `Mouse ID`
- Remove duplicate mouse records
- Validate data integrity before analysis

---

### 2) Summary Statistics
- Compute mean, median, variance, standard deviation, and SEM
- Group statistics by **drug regimen**
- Identify regimens with lower average tumor volumes

---

### 3) Data Visualization
- **Bar charts**
  - Total number of observations per drug regimen
- **Pie charts**
  - Distribution of mice by sex
- **Line plots**
  - Tumor volume over time for individual mice treated with Capomulin
- **Box plots**
  - Tumor volume distributions for top-performing drug regimens

---

### 4) Statistical Analysis
- **Outlier detection** using IQR
- **Linear regression**
  - Tumor volume vs mouse weight (Capomulin)
- **Correlation analysis**
  - Evaluates relationship between mouse weight and tumor volume

---

## Key Findings
- Capomulin and Ramicane show the **lowest average tumor volumes**
- Tumor volume generally **increases with mouse weight**
- Capomulin demonstrates consistent tumor volume reduction over time for individual mice
- Weight is strongly correlated with tumor volume under Capomulin treatment

---

## Key Concepts Demonstrated
- Data cleaning and merging
- Grouped statistical analysis
- Exploratory data analysis (EDA)
- Regression modeling and correlation
- Scientific data visualization
- Reproducible analytical workflows
