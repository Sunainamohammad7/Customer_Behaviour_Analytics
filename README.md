# Customer_Behaviour_Analytics
A complete end-to-end data analytics project where I loaded and cleaned customer data in Python, performed exploratory analysis, validated insights using SQL in MySQL, and built an interactive Power BI dashboard to understand customer spending patterns, revenue distribution, and subscription behavior.

# 🧾 Customer Behaviour Dashboard

### **Overview**
This project demonstrates a complete **Data Analytics workflow** — from data loading and cleaning in Python to performing SQL analysis in MySQL and designing an interactive **Power BI dashboard**. The analysis helps understand customer purchase trends, subscription behavior, and revenue drivers.

---

### **Project Workflow**

#### **1. Data Loading (Python)**
- Loaded the dataset using `pandas` and performed initial data checks.
- Cleaned missing and inconsistent data for accurate results.

import pandas as pd

df = pd.read_csv("customer_behaviour.csv")
df.info()
df.drop_duplicates(inplace=True)
df.fillna(0, inplace=True)

### **2. Exploratory Data Analysis (EDA)

Performed statistical analysis to understand trends and distributions.

Generated insights on purchase amounts, age groups, and customer subscriptions.

Visualized findings using matplotlib and seaborn for better clarity.

Key Insights:

Most customers belong to the Young Adult and Adult age groups.

Clothing generates the highest revenue and sales volume.

About 27% of customers have an active subscription.

### **3. SQL Analysis (MySQL)

Imported the cleaned data into MySQL for analytical queries.

Validated and aggregated insights using SQL.

SELECT category, SUM(revenue) AS total_revenue
FROM customer_behaviour
GROUP BY category
ORDER BY total_revenue DESC;


SQL Tasks:

Compared average purchase values by subscription type.

Identified top-performing product categories.

Aggregated revenue by age and gender for deeper segmentation.

4. Dashboard Creation (Power BI)

Connected MySQL data to Power BI.

Designed a clean, interactive dashboard showing:

Total Customers

Average Purchase Amount

Average Review Rating

Revenue by Category

Sales by Age Group

Customer Subscription Split

Dashboard Features:

Filters by Gender, Subscription Status, and Shipping Method.

Charts for Revenue & Sales comparisons.

Dynamic KPIs summarizing key metrics.

Tools & Technologies

Python: Pandas, NumPy, Matplotlib, Seaborn

Database: MySQL

Visualization: Power BI

Environment: Jupyter Notebook

Key Takeaways:

Learned end-to-end data pipeline: loading → cleaning → SQL → dashboarding.

Improved storytelling with data through visualization.

Delivered actionable insights for business decision-making.

Screenshot of Dashboard: 

Example of Dashboard : https://github.com/Sunainamohammad7/Customer_Behaviour_Analytics/blob/main/Customer_Behaviour.pbix 

