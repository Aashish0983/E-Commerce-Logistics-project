# E-Commerce-Logistics-project
Python-based e-commerce logistics analysis to validate courier charges by calculating shipment weight, weight slabs, delivery zones, and expected freight, then identifying overcharged, correctly charged, and undercharged orders.

# 🚚 E-commerce Logistics & Courier Charge Analysis

## 📌 Project Overview

This project analyzes courier charges for an e-commerce company, **ShopX**, using Python.

The main objective is to verify whether courier companies are charging the correct amount for each order based on **product weight, weight slabs, delivery zones, freight type, and courier rate cards**.

The project compares the expected shipping charges calculated by ShopX with the actual charges billed by the courier company.

## 🎯 Project Objective

The project aims to:

- Calculate the total weight of each order
- Determine the applicable weight slab
- Identify the correct delivery zone
- Calculate expected courier charges
- Compare expected charges with billed charges
- Identify overcharged and undercharged orders
- Prepare order-level and summary-level reports

## 🛠️ Tools & Technologies

- **Python**
- Pandas
- NumPy
- Excel
- CSV
- Data Cleaning
- Data Analysis
- Business Logic

## 🔍 Analysis Process

### 1️⃣ Order Data Analysis

Used ShopX order data containing:

- Order ID
- Product Code
- Units Ordered

### 2️⃣ Product Weight Calculation

Used product weight data to calculate the **total shipment weight for each order**.

```text
Total Weight = Product Weight × Units Ordered
```
### 3️⃣ Weight Slab Calculation

Converted total shipment weight into the applicable 0.5 KG weight slab.

Examples:

400 g   → 0.5 KG
950 g   → 1.0 KG
1.0 KG  → 1.0 KG
2.2 KG  → 2.5 KG

### 4️⃣ Delivery Zone Calculation

Used warehouse pincode and customer area code to determine the applicable delivery zone and compared it with the zone reported by the courier company.

### 5️⃣ Expected Charge Calculation

Applied the courier rate card based on:

Delivery Zone
Weight Slab
Fixed Charges
Additional Weight Charges
Freight Type
RTO Charges

### 6️⃣ Charge Comparison

Compared:

Expected Charge vs Courier Billed Charge

and calculated the difference for every order.

### 📊 Final Output
```text
The order-level analysis contains:

Order ID
AWB Number
Total Weight as per ShopX
Weight Slab as per ShopX
Total Weight as per Courier
Weight Slab Charged by Courier
Delivery Zone as per ShopX
Delivery Zone Charged by Courier
Expected Charge
Courier Billed Charge
Difference in Charges
```

### 📈 Summary Analysis
```text
Orders are classified into:

Category	Description
✅ Correctly Charged	Expected charge matches billed charge
🔴 Overcharged	Courier billed more than expected
🟢 Undercharged	Courier billed less than expected

The summary report provides the order count and total amount for each category.
```

### 💡 Business Value
```text
This analysis helps ShopX:

Identify courier overcharging
Validate courier invoices
Detect incorrect weight or zone calculations
Monitor shipping costs
Reduce unnecessary logistics expenses
Improve courier billing accuracy
```
## 📁 Project Structure

```text
Ecommerce-Logistics-Analysis/
│
├── Data/
│   ├── Order_Data.csv
│   ├── Product_Weight.csv
│   ├── Pincode_Zone.csv
│   ├── Courier_Invoice.csv
│   └── Courier_Rates.csv
│
├── Python/
│   └── Logistics_Charge_Analysis.py
│
├── Output/
│   ├── Order_Level_Calculation.xlsx
│   └── Summary_Report.xlsx
│
├── Documentation/
│   └── Logistics_Assignment_Problem.pdf
│
└── README.md
```
## 🔄 Project Workflow
```text
Raw Data
    ↓
Data Cleaning
    ↓
Merge Multiple Data Sources
    ↓
Calculate Total Order Weight
    ↓
Calculate Weight Slab
    ↓
Determine Delivery Zone
    ↓
Calculate Expected Courier Charge
    ↓
Compare With Billed Charge
    ↓
Identify Overcharged / Undercharged Orders
    ↓
Generate Excel Reports
    ↓
Business Insights
```

### 👨‍💻 Project By

**Aashish Lovewanshi** -
Data Analyst | Adv Excel | Google Sheets | SQL | Python | Power BI | Machine Learning | Meaningful Insights


## 📬 Connect With Me

**Aashish Lovewanshi**

💼 Data Analyst

* 🔗 LinkedIn: https://www.linkedin.com/in/aashish-lovewanshi/
* 💻 GitHub: [https://github.com/aashishlovewanshi](https://github.com/Aashish0983)

---

### ⭐ If you found this project helpful or interesting, consider giving it a **Star**. Your support motivates me to build more data analytics projects!
