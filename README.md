# RFM-Analysis-Project


## 📌 Project Overview
This project applies **RFM Analysis (Recency, Frequency, Monetary)** to segment customers of a UK-based online retail store.  
The goal is to **identify high-value customers** and provide **data-driven marketing strategies** for retention and reactivation.

**Niche:** E-Commerce  
**Dataset:** [UCI Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)  
**Tools Used:Python (data cleaning), Tableau (visualization)

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
### 1. **Data Cleaning (Python)**
- Removed rows with missing `CustomerID`
- Removed returns (negative `Quantity`)
- Checked for invalid prices
- Added `Line_Total = Quantity * UnitPrice`

### 2. **RFM Metrics**
- **Recency:** Days since last purchase  
- **Frequency:** Total number of purchases  
- **Monetary:** Total spending per customer  

### 3. **Scoring & Segmentation (Python)**
- Scored each metric from **1 (lowest)** to **5 (highest)**  
- Combined scores into RFM codes (e.g., `555` = Champions)  
- Segmented into categories:
  - **Champions**
  - **Loyal Customers**
  - **New Customers**
  - **At Risk**

### 4. **Visualization**
- Tableau: Several sheets for customer info. Other sheets for further customer analysis.

---

## 📈 Visual Previews
### Tableau Dashboard?
🔗 [View Customers Sales Preferences](https://public.tableau.com/views/RFMAnalysis_17547504359310/Sheet10?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 

---

## 📜 License
This project is for educational and portfolio purposes. Dataset provided by the [UCI Machine Learning Repository](https://archive.ics.uci.edu).

---
