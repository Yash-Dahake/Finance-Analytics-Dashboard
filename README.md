# 📊 Finance Analytics Dashboard

An interactive **Finance Analytics Dashboard** built using **Power BI** to analyze financial transactions, customer behavior, transaction performance, fees, taxes, and regional trends.

## 📌 Project Overview

This dashboard provides a centralized view of financial performance and helps stakeholders:

- Monitor KPIs and YoY performance
- Analyze monthly transaction trends
- Compare Success, Failed, and Pending transactions
- Identify high-value customer segments
- Compare state-wise performance
- Analyze transaction types, fees, and taxes
- Explore customer demographics
- Drill through to detailed transaction records
## 📸 Dashboard Preview

### Executive Finance Analysis

![Finance Analysis Dashboard](Screenshot%20_Preview_Analysis.png)

### Transaction Details

![Transaction Details Dashboard](Screenshot%20_Transaction.png)

## 🎛️ Dashboard Filters

- Year
- Dynamic Measure
- Occupation
- Category

The **Dynamic Measure** selector allows analysis of:
- Total Amount
- Total Fees
- Total Tax
- Total Transactions

## 📊 Dashboard Visuals

| Visual | Chart Type |
|---|---|
| Total Amount by Month | Area / Line Chart |
| Amount by Transaction Status | Donut Chart |
| Amount by Customer Segment | Bar Chart |
| Amount by State | Bar Chart |
| Transaction Type Analysis | Matrix / Heatmap |
| Amount by Gender | Donut Chart |
| Transaction Details | Table / Grid |

## 📌 Key KPIs

- **Total Amount**
- **Total Transactions**
- **Average Transaction Value**
- **Total Fees**
- **Total Tax**
- **YoY Performance**

## 🔍 Drill-through Analysis

The second dashboard page provides detailed transaction-level records.

```text
Dashboard Analysis
       ↓
Select Category / State / Transaction Type
       ↓
Drill Through
       ↓
Transaction Details
🛠️ Tech Stack
Power BI Desktop
Power Query (M)
DAX
Data Modeling
CSV
📂 Dataset
finance_transactions.csv

Contains transaction details such as amount, fees, tax, transaction type, status, and date.

customers.csv

Contains customer information such as segment, occupation, gender, and state.

📐 Key DAX
Total Amount =
SUM(finance_transactions[Transaction_Amount])

Total Transactions =
COUNTROWS(finance_transactions)

Avg Transaction Value =
DIVIDE(
    [Total Amount],
    [Total Transactions],
    0
)

Total Fees =
SUM(finance_transactions[Fee_Amount])

Total Tax =
SUM(finance_transactions[Tax_Amount])
📁 Repository Structure
Finance-Analytics-Dashboard/
│
├── Finance_dashboard.pbix
├── README.md
├── Screenshot_Preview_Analysis.png
├── customers.csv
└── finance_transactions.csv
🚀 How to Run
Clone the repository.
Open Finance_dashboard.pbix in Power BI Desktop.
Update the CSV file paths if required.
Refresh the data.
Use the filters and drill-through features to explore the dashboard.
👨‍💻 Author

Yash Dahake

Data Analyst | Power BI | SQL | Python | Excel

⭐ Project Highlights
Interactive Power BI Dashboard
Dynamic Measures
KPI & YoY Analysis
Customer & Regional Analysis
Transaction Status Analysis
Matrix / Heatmap
Drill-through Details
Business-focused Insights
📌 Disclaimer

This project is created for educational and portfolio purposes. The financial data is used for analytical practice and does not represent confidential information from any financial institution.
