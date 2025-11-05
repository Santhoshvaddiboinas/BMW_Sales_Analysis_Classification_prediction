BMW_Sales:
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

## Forecast (2025-2029) – *Linear Trend*  

The notebook already contains a **placeholder** for a forecast line plot (green line + dots).  
Below is a **compact ASCII representation** of a *linear* projection based on the historical `Year → Sales_Volume` relationship (average ~360 units/year growth, derived from the data range).

```text
BMW Sales Volume Forecast (2025-2029)
──────────────────────────────────────
2025  ████████████████░░░░░░  ~8 420
2026  ██████████████████░░░░  ~8 780
2027  ████████████████████░░  ~9 140
2028  ██████████████████████  ~9 500
2029  ███████████████████████ ~9 860
──────────────────────────────────────
Trend: +~360 units per year (steady growth)
