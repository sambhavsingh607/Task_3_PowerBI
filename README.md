# Sales Performance Dashboard Project 🚀

## 1. Project Overview

This repository documents the creation of a fully **Interactive Sales Performance Dashboard** using Power BI. The goal was to transform raw sales data into actionable business intelligence, fulfilling all requirements of the project brief.

| Feature | Status |
| :--- | :--- |
| **Tool Used** | Power BI Desktop |
| **Deliverables** | Power BI Report File (`.pbix`) |
| **Objective** | Analyze sales trends, measure KPIs, and inform strategic decisions. |

---

## 2. Dashboard Screenshot

The final dashboard layout implements **KPI cards**, **Slicers** for interactivity, **Time-Series analysis**, and **Categorical Breakdowns** by product and geography.



---

## 3. Data Source & Preparation

The analysis was conducted on the `sales_data_sample.csv` file, with critical data preparation performed in Power Query.

* **File:** `sales_data_sample.csv`
* **Key Preparation Steps:**
    * **Data Type Conversion:** Successfully converted the `ORDERDATE` column to a **Date/Time** type using **Locale (English US)** to handle the date format ambiguity.
    * **Time Dimensions:** Extracted **Year**, **Month Name**, and **Quarter** columns to enable robust time-series charting.

---

## 4. Key Performance Indicators (KPIs)

The following core business metrics were calculated using **DAX Measures** and prominently displayed on KPI cards:

| KPI | DAX Formula | Description |
| :--- | :--- | :--- |
| **Total Sales** | `SUM('sales_data_sample'[SALES])` | Total Revenue generated. |
| **Total Orders** | `DISTINCTCOUNT('sales_data_sample'[ORDERNUMBER])` | Total unique transactions (Order Volume). |
| **Average Order Value (AOV)** | `DIVIDE([Total Sales], [Total Orders])` | Revenue efficiency per order. |
| **Quantity Sold** | `SUM('sales_data_sample'[QUANTITYORDERED])` | Total units moved. |

---

## 5. Visualizations and Interactivity

The dashboard utilizes a strategic set of visuals to facilitate detailed drill-down analysis.

| Category | Visual Type | Key Fields | Function |
| :--- | :--- | :--- | :--- |
| **Time Series** | Line Chart | `Month Name`, `Year`, `[Total Sales]` | Tracks **Year-over-Year growth and seasonality.** |
| **Breakdowns** | Bar, Map, Donut | `PRODUCTLINE`, `COUNTRY`, `DEALSIZE` | Identifies **top revenue drivers and geographic concentration.** |
| **Slicers** | Vertical List/Dropdown | `YEAR_ID`, `COUNTRY`, `PRODUCTLINE` | Allows instant, interactive filtering of all report visuals. |

---

## 6. Project Outcome and Conclusion

The project successfully delivered a fully functional, stakeholder-ready dashboard, meeting all original requirements.

### 🎯 Key Insights for Stakeholders:

* **Peak Seasonality:** Analysis confirms a strong sales cycle, peaking predictably in Q4.
* **Product Focus:** The top 3 `PRODUCTLINE`s are identified as core revenue drivers, justifying prioritized investment.
* **AOV Efficiency:** The **Average Order Value** provides a key metric for evaluating sales efficiency across different customer segments.

### 🧠 Skills Demonstrated:

* **Advanced Data Prep:** Overcame data type errors using **Power Query's Locale** settings.
* **DAX Modeling:** Implemented fundamental and conditional measures.
* **Visualization & UX:** Designed an aesthetically pleasing and user-friendly interface for executive-level consumption.

---

## 7. Getting Started

To view or fork this project:

1.  **Download** Power BI Desktop.
2.  **Clone** this repository and ensure the `sales_data_sample.csv` file is accessible in the same directory.
3.  **Open** the main Power BI Report file (`<Your Project Name>.pbix`).

   <img width="1143" height="645" alt="image" src="https://github.com/user-attachments/assets/5bf648f7-3a40-40b7-aaf8-65f635860906" />
