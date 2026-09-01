# ShadowFox Data Analyst Internship - Beginner Level Project

## 📌 Project Overview
This repository contains the complete submission for the **Beginner Level Data Analyst Track** at **ShadowFox**. The project evaluates raw Q1 2026 sales transaction data to monitor operational KPIs, categorical profitability, regional distribution, and monthly revenue trends.

![Dashboard Preview](dashboard_screenshot.png)

---

## 🛠️ Data Hygiene & Calculated Fields

### 1. Data Cleaning & Validation
- **Standardization:** Validated transaction dates into `YYYY-MM-DD` standard format and set monetary fields to standard USD currency formatting (`$`).
- **Calculated Columns:**
  - `Revenue ($)` = `=F2*G2` (*Units Sold × Unit Price*)
  - `Profit ($)` = `=H2-I2` (*Revenue − Cost*)
- **Data Integrity:** Verified zero missing fields, duplicated transaction IDs, or illegal numerical inputs.

### 2. Core Metrics (KPIs)
- **Total Sales Revenue:** `$61,550.00` (`=SUM(H2:H13)`)
- **Total Net Profit:** `$17,860.00` (`=SUM(J2:J13)`)
- **Overall Profit Margin:** `29.02%` (`=SUM(J2:J13)/SUM(H2:H13)`)
- **Total Units Sold:** `405 Units` (`=SUM(F2:F13)`)
- **Average Order Value (AOV):** `$5,129.17` (`=AVERAGE(H2:H13)`)

---

## 📊 Summary Performance Tables

### Category Performance Breakdown
| Category | Revenue ($) | Profit ($) | Profit Margin (%) |
| :--- | :--- | :--- | :--- |
| **Electronics** | $42,100.00 | $12,150.00 | 28.86% |
| **Furniture** | $5,450.00 | $2,050.00 | 37.61% |
| **Office Supplies** | $1,600.00 | $910.00 | 56.88% |

### Monthly Trend Analysis (Q1 2026)
| Month | Revenue ($) | Units Sold | Movement Trend |
| :--- | :--- | :--- | :--- |
| **January** | $23,250.00 | 150 | Peak Volume |
| **February** | $22,500.00 | 112 | Steady (-3.2%) |
| **March** | $15,800.00 | 143 | Contraction (-29.7%) |

---

## 💡 Key Business Observations

1. **Top-Line Concentration:** **Electronics** is the key revenue driver, producing **$42,100 (68.4%)** of total quarterly revenue, driven primarily by high-ticket Laptops and Phones.
2. **Margin Profile Asymmetry:** **Office Supplies** yields lower aggregate sales ($1,600), but delivers the highest relative profit margin (**56.88%**).
3. **Late-Quarter Volatility:** Monthly revenues contracted by 32% from January ($23,250) to March ($15,800), pointing to end-of-quarter volume slowdowns.

---

## 🚀 Actionable Business Recommendations

1. **Focus Marketing on Core Drivers:** Increase ad spend on high-ticket Electronics items to maintain strong top-line sales.
2. **Cross-Sell High-Margin Office Supplies:** Create promotional bundles pairing low-cost, high-margin items (Paper, Binders) with primary Electronics purchases to boost Average Order Value.
3. **Late-Quarter Sales Incentives:** Implement targeted mid-to-late quarter discount campaigns to counteract March volume drops.

---

## 📁 Repository Contents
- `ShadowFox_Beginner_Dashboard.xlsx` — Excel workbook containing raw data, KPI metrics, and formulas.
- `ShadowFox_Internship_Report.docx` — Executive 2-page project report document.
- `dashboard_screenshot.png` — Visual chart screenshot previewing key dataset insights.
