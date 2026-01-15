# Day 2 – Anomaly Report
**Dataset:** Online Retail - Kaggle  
**Date:** 2025-08-13 
**Analyst:** Ayisha Liya

---

## 1. Purpose
The goal of this report is to document unusual or suspicious values in the cleaned dataset before proceeding to analysis.

---

## 2. Summary of Findings
| Type of Anomaly        | Description                       | Example(s)                    | Possible Cause                   | Action Taken       |
|------------------------|-----------------------------------|-------------------------------|----------------------------------|--------------------|
| Negative Quantity      | Rows with Quantity < 0            | Invoice #C536379	             | Product returns or cancellations | Removed            |
| Extreme Quantity       | Quantity > 1000                   | Invoice #581483 – 80995 units | Bulk wholesale order or error    | Flagged for review |
| Negative UnitPrice     | UnitPrice < 0                     | N/A                           | Data entry error                 | Removed            |
| Unusually High Price   | UnitPrice > £500                  | Invoice #551697 – £8142.75    | Pricing error or special item    | Flagged            |
| Missing Country        | Country field blank/unspecified   | CustomerID 12363              | Data issue                       | Removed            |
| Out-of-range Dates     | Dates outside Dec 2010–Dec 2011   | N/A                           | Data entry issue                 | Removed            |
| Non product items      | Items with StockCode POST, DOT, M | Invoice #551697	             | Data issue                       | Removed            |
| Negligible UnitPrice   | UnitPrice with £0 to £0.5         | Invoice #537197               | Data entry issue                 | Removed            |


---