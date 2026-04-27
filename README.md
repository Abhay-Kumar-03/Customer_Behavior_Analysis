# 🛍️ Customer Shopping Behavior Analysis

## 📌 Overview

This project analyzes retail customer shopping behavior to uncover revenue patterns, customer segments, and product performance. The goal is to generate actionable business recommendations that help improve subscriptions, loyalty, and targeted marketing.

The project follows a full analytics workflow — from raw data ingestion to a polished Power BI dashboard and executive presentation.

---

# DASHBOARD 
<img width="1920" height="984" alt="CBD1" src="https://github.com/user-attachments/assets/aab1f4b5-612c-4a84-aceb-c4ea3a9a1943" />

<img width="1920" height="981" alt="CBD2" src="https://github.com/user-attachments/assets/15184894-74f3-4941-9062-38768185e874" />

<img width="1920" height="973" alt="CBD3" src="https://github.com/user-attachments/assets/6b90de63-3c66-4d00-b15d-56c7c5f47f7e" />

<img width="1920" height="974" alt="CBD4" src="https://github.com/user-attachments/assets/b8a5d9d1-daff-404a-bee1-c24fb79b63d1" />

<img width="1920" height="981" alt="CBD5" src="https://github.com/user-attachments/assets/f16e20aa-5ee8-4db2-94d0-921ec6daee82" />

<img width="1920" height="982" alt="CBD6" src="https://github.com/user-attachments/assets/2ebbc94c-dd7e-4683-8292-9e2e80ecda0d" />





> End-to-end data analytics project covering Python, SQL Server, Power BI, and business reporting  
> **3,900 transactions · 18 features · 50 locations**

---



## 📂 Dataset

| Property | Details |
|---|---|
| Source | Customer Shopping Dataset (Kaggle) |
| Rows | 3,900 transactions |
| Features | 18 columns |
| Missing Values | 37 (Review Rating column) |
| Coverage | 50 US locations |

**Key columns:** `customer_id`, `age`, `gender`, `category`, `purchase_amount`, `subscription_status`, `shipping_type`, `review_rating`, `frequency_of_purchases`

---

## 🛠️ Tools & Technologies

| Layer | Tool |
|---|---|
| Data Cleaning & EDA | Python (Pandas, Matplotlib, Seaborn) |
| Database | SQL Server (SSMS) |
| Visualization | Power BI |
| Reporting | MS Word / PDF |
| Presentation | PowerPoint (Gamma) |
| Version Control | Git & GitHub |

---

## 🔄 Project Steps

### 1. 🐍 Data Preparation in Python
- Loaded raw CSV using Pandas
- Imputed 37 missing `review_rating` values using **median by category**
- Renamed all columns to `snake_case` for consistency
- Engineered two new features: `age_group` and `purchase_frequency_days`
- Exported cleaned data to SQL Server via `pyodbc` / `sqlalchemy`

### 2. 🗄️ SQL Analysis (SQL Server)
- Queried revenue by gender, category, and subscription status
- Segmented customers into **Loyal**, **Returning**, and **New** using purchase frequency
- Ranked top products by average review rating
- Compared shipping type performance (Express vs. Standard)
- Identified discount-heavy products by discount application rate

### 3. 📊 Power BI Dashboard
- Connected Power BI directly to SQL Server
- Built interactive visuals: bar charts, KPI cards, slicers by gender/category/age
- Added dynamic titles and cross-filter relationships between visuals
- Published dashboard with 4 core KPIs: Total Customers, Avg Purchase, Avg Rating, Subscriber Rate

### 4. 📝 Report & Presentation
- Summarized findings in a structured business report
- Created an executive PowerPoint covering dataset overview, key insights, and recommendations

---

## 📈 Dashboard KPIs

| Metric | Value |
|---|---|
| Total Customers | 3,900 |
| Average Purchase Amount | $59.76 |
| Average Review Rating | 3.75 / 5 |
| Subscriber Rate | 27% |

---

## 💡 Key Results

- **Male customers** generated 2.1× more revenue than female customers ($157,890 vs. $75,191)
- **80% of customers** fall in the Loyal segment — strong retention, weak new acquisition
- Subscribers and non-subscribers have nearly **identical average spend** ($59.87 vs. $59.49), suggesting subscription drives volume, not ticket size
- **Clothing** is the top revenue category; **Gloves** rank #1 by review rating (3.86 avg)
- **Hat, Sneakers, and Coat** are the most discounted products (~50% discount rate)
- Express shipping customers spend slightly more on average ($60.48 vs. $58.46)

---

## 📋 Business Recommendations

1. **Boost Subscriptions** — Promote exclusive subscriber benefits to grow the 27% subscriber base
2. **Loyalty Programs** — Reward the existing 80% loyal customer segment to increase spend per visit
3. **Review Discount Policy** — High discount rates on Hats and Sneakers may be eroding margins
4. **Targeted Marketing** — Focus campaigns on Young Adults (top revenue age group) and Express shipping users

---

## 🚀 How to Run

### Prerequisites
```
Python 3.8+
SQL Server / SSMS
Power BI Desktop
```

### Step 1 — Clone the repo
```bash
git clone https://github.com/Abhay-Kumar-03/Customer_Behavior_Analysis.git
cd customer-shopping-analysis
```

### Step 2 — Install Python dependencies
```bash
pip install pandas matplotlib seaborn sqlalchemy pyodbc
```

### Step 3 — Run the Python notebook
```bash
jupyter notebook notebooks/eda_cleaning.ipynb
```

### Step 4 — Load data to SQL Server
Update the connection string in `scripts/load_to_sql.py` with your server credentials, then run:
```bash
python scripts/load_to_sql.py
```

### Step 5 — Run SQL queries
Open `sql/analysis_queries.sql` in SSMS and execute against your database.

### Step 6 — Open Power BI Dashboard
Open `dashboard/customer_shopping.pbix` in Power BI Desktop and refresh the data source connection.

---

## 📁 Folder Structure

```
customer-shopping-analysis/
│
├── data/
│   ├── raw/                  # Original CSV dataset
│   └── cleaned/              # Cleaned CSV after Python processing
│
├── notebooks/
│   └── eda_cleaning.ipynb    # EDA and data cleaning notebook
│
├── scripts/
│   └── load_to_sql.py        # Script to load data into SQL Server
│
├── sql/
│   └── analysis_queries.sql  # All SQL queries used in analysis
│
├── dashboard/
│   └── customer_shopping.pbix  # Power BI dashboard file
│
├── report/
│   └── analysis_report.pdf   # Final business report
│
├── presentation/
│   └── project_presentation.pdf  # Executive slide deck
│
└── README.md
```

---

## 👤 Author

**Abhay**  
Aspiring Data Analyst | Python · SQL · Power BI ·Excel 
📧 abhaychauhan8052@gmail.com  
🔗 [LinkedIn]([https://linkedin.com/in/your-profile](https://www.linkedin.com/in/abhay-kumar-304462229/)) 
    [GitHub]([https://github.com/your-username](https://github.com/Abhay-Kumar-03))

---


