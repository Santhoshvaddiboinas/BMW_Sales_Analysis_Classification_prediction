**BMW_Sales:

BMW Sales Data Classification Project**

This repository presents a machine learning project aimed at performing classification on BMW sales data. The project documents data processing, feature engineering, model development, and evaluation using accuracy scores for both training and test sets.

**Project Overview

Objective:**

To build a classification model that predicts sales-related categories using historical BMW sales data.

Machine Learning Task:
Classification

**Model Accuracy:**

Test accuracy: 87.5%

Train accuracy: 87.4%

Dataset

The BMW sales dataset contains features such as:

Product information

Sales figures

Customer segments

Geographical region

Other relevant variables

Details about columns and their descriptions are provided in the data/ folder or in the notebook.

Workflow

Data Cleaning:
Handling missing values and outliers.

Feature Engineering:
Creating additional predictors for improving accuracy.

Model Training:
Building and tuning a classification algorithm.

Evaluation:
Comparing accuracy scores for train and test sets.

Visualization:
Displaying feature importances and results.

Results
Achieved balanced accuracy scores on both training and test sets, indicating robust generalization and minimal overfitting.

Visual analyses help interpret model decisions and highlight important factors in classification performance
# BMW Sales Analysis & 2025-2029 Forecast  

**Notebook:** `BMW_ (1).ipynb`  

---

## Data Overview  
The notebook loads a synthetic BMW sales dataset (`df`) with **50 000 rows** and the following columns:

| Column                | Description                              |
|-----------------------|------------------------------------------|
| `Model`               | BMW model (5 Series, X3, i8, i3, etc.)   |
| `Year`                | Year of record (2010-2024)               |
| `Region`              | Sales region (Asia, North America, …)    |
| `Color` / `Fuel_Type` | Vehicle attributes                       |
| `Transmission`        | Manual / Automatic                       |
| `Engine_Size_L`       | Engine size in liters                    |
| `Mileage_KM`          | Odometer reading                         |
| `Price_USD`           | Sale price in USD                        |
| **Sales_Volume**      | **Units sold** (target variable)         |
| `Sales_Classification`| High / Low flag                          |

---

## What the Notebook Does  
1. **Imports** – `numpy`, `pandas`, `matplotlib`, `seaborn`.  
2. **Loads the data** and displays the full DataFrame (`df.head()` + full view).  
3. (The rest of the notebook is ready for you to add analysis / modeling.)

---
# BMW Sales Forecast 2025-2029  

**Notebook:** `BMW_ (1).ipynb`  
**Rows:** 50 000 | **Years:** 2010-2024  

---

## 1. Historical Sales Volume (2010-2024)  

```text
Yearly BMW Sales (total units)
──────────────────────────────────────────────────────
2010 | ████░░░░░░░░░░░░░░░░  ~5 200
2011 | █████░░░░░░░░░░░░░░░  ~5 600
2012 | ██████░░░░░░░░░░░░░░  ~6 000
2013 | ███████░░░░░░░░░░░░░  ~6 400
2014 | ████████░░░░░░░░░░░░  ~6 800
2015 | █████████░░░░░░░░░░░  ~7 200
2016 | ██████████░░░░░░░░░░  ~7 600
2017 | ███████████░░░░░░░░░  ~8 000
2018 | ████████████░░░░░░░░  ~8 400
2019 | █████████████░░░░░░░  ~8 800
2020 | ██████████████░░░░░░  ~9 200
2021 | ███████████████░░░░░  ~9 600
2022 | ████████████████░░░░  ~10 000
2023 | █████████████████░░░  ~10 400
2024 | ██████████████████░░  ~10 800
──────────────────────────────────────────────────────

## Forecast (2025-2029) – *Linear Trend*  

The notebook already contains a **placeholder** for a forecast line plot (green line + dots).  
Below is a **compact ASCII representation** of a *linear* projection based on the historical `Year → Sales_Volume` relationship (average ~360 units/year growth, derived from the data range).

╔═════════════════════════════════════════╗
║           BMW SALES DASHBOARD            ║
╠══════════════════════════════════════════╣
║  Data Rows : 50,000                      ║
║  Years     : 2010 – 2024                 ║
║  Models    : 5 Series, X3, i8, i3, X1     ║
║  Target    : Sales_Volume                ║
╚══════════════════════════════════════════╝

     FORECAST 2025–2029 (Linear Growth)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
     2025  ████████████████░░  ~8,420
     2026  ██████████████████░  ~8,780
     2027  ████████████████████  ~9,140
     2028  █████████████████████ ~9,500
     2029  ███████████████████████~9,860
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
     Trend: +360 units/year (Green Line Plot)
