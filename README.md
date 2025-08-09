# RFM-Analysis-Project


## 📌 Project Overview
This project applies **RFM Analysis (Recency, Frequency, Monetary)** to segment customers of a UK-based online retail store.  
The goal is to **identify high-value customers** and provide **data-driven marketing strategies** for retention and reactivation.

**Niche:** E-Commerce  
**Dataset:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)  
**Tools Used:** Excel (main analysis), Tableau (visualization), Python (optional preprocessing)  

---

## 🎯 Business Objective
Segment the customer base to answer:
1. Who are the most frequent and highest-spending customers?
2. How recently have they shopped?
3. What tailored offers could retain or re-engage them?

---

## 📂 Dataset Details
- **Transactions:** Dec 2010 – Dec 2011
- **Key Columns:**  
  - `InvoiceNo` – Unique invoice number  
  - `StockCode` – Product code  
  - `Description` – Product description  
  - `Quantity` – Number of units purchased  
  - `InvoiceDate` – Purchase date/time  
  - `UnitPrice` – Price per unit (£)  
  - `CustomerID` – Unique customer ID  
  - `Country` – Country of customer  

---

## 🛠️ Methodology
### 1. **Data Cleaning (Excel)**
- Removed rows with missing `CustomerID`
- Removed returns (negative `Quantity`)
- Checked for invalid prices
- Added `Line_Total = Quantity * UnitPrice`

### 2. **RFM Metrics**
- **Recency:** Days since last purchase  
- **Frequency:** Total number of purchases  
- **Monetary:** Total spending per customer  

### 3. **Scoring & Segmentation**
- Scored each metric from **1 (lowest)** to **5 (highest)**  
- Combined scores into RFM codes (e.g., `555` = Champions)  
- Segmented into categories:
  - **Champions**
  - **Loyal Customers**
  - **New Customers**
  - **At Risk**
  - **Churned**

### 4. **Visualization**
- Excel: Pivot tables, conditional formatting, charts
- Tableau: Interactive segmentation dashboard

---

## 📊 Key Insights
- **Champions** (R=5, F=5, M=5) contributed **X% of total revenue** while representing only **Y% of customers**.
- **At Risk** customers have high historical spending but haven’t purchased in over **Z days**.
- Tailored retention campaigns for **Loyal Customers** could significantly improve repeat purchases.

---

## 📈 Visual Previews
### Tableau Dashboard
🔗 [View Customers Sales Preferences](https://public.tableau.com/views/RFMAnalysis_17547504359310/Sheet10?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 

![RFM Segmentation Example](images/rfm_segments.png)

---

## 💡 Business Recommendations
- **Champions:** Loyalty rewards & exclusive offers
- **At Risk:** Win-back discounts & personalized emails
- **New Customers:** Onboarding with product recommendations

---

## 📥 Project Files
- 📊 [Excel Analysis File](excel/RFM_Analysis.xlsx)
- 📄 [Full PDF Report](report/RFM_Analysis_Report.pdf)
- 💻 [Python Data Cleaning Script](python/data_cleaning.py)

---

## 📌 How to Reproduce
1. Download the dataset from [UCI Repository](https://archive.ics.uci.edu/dataset/352/online+retail)
2. Open the Excel file in `/excel` folder
3. Follow the same pivot table and scoring steps as documented in the report

---

## 📜 License
This project is for educational and portfolio purposes. Dataset provided by the [UCI Machine Learning Repository](https://archive.ics.uci.edu).

---
