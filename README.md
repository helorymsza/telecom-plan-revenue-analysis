# Telecom Plan Revenue Analysis

## Overview
This project is an analytical case study for a telecom company, **Megaline**, which offers two prepaid plans: **Surf** and **Ultimate**.  
The goal of this project is to analyze customer behavior and determine which plan generates more revenue on average.  

The analysis is based on **500 customers** and includes their calls, messages, internet usage, and plan details for 2018. Statistical tests and visualizations are used to explore the data.

---

## Datasets
The project uses the following datasets:

- `megaline_users.csv` – Information about users (ID, name, age, city, plan, churn date).  
- `megaline_calls.csv` – Call records (user ID, call duration, date).  
- `megaline_messages.csv` – Messages sent (user ID, date).  
- `megaline_internet.csv` – Internet usage (user ID, session date, MB used).  
- `megaline_plans.csv` – Plan details (price, included minutes/messages/MB, overage fees).

---

## Key Steps in Analysis

1. **Data Overview & Cleaning**
   - Loaded all datasets into Pandas DataFrames.
   - Checked data types, missing values, and cleaned inconsistencies.
   - Created new columns to categorize users as `Active` or `Inactive`.

2. **Data Aggregation**
   - Aggregated user data per month: number of calls, minutes used, messages sent, and internet usage (in GB).  
   - Calculated monthly revenue per user based on their plan and overage charges.

3. **Data Exploration**
   - Explored statistics per plan: mean, variance, and standard deviation.
   - Created histograms to visualize distributions of usage and revenue.

4. **Hypothesis Testing**
   - Tested whether average revenue differs between **Surf** and **Ultimate** plans.  
   - Tested whether revenue differs for customers in the **NY-NJ area** versus other regions.

5. **Conclusions**
   - Surf plan is cheaper with lower included minutes, messages, and data.  
   - Ultimate plan is more expensive but includes more services.  
   - Statistical analysis showed which plan generates more revenue and insights about geographic differences in customer usage.

---

## 🚀 How to Run Locally

1. **Clone the repository:**

<pre> ## How to Run Locally 
   
   1. **Clone the repository:** 
   
   ```bash git clone https://github.com/helorymsza/telecom-plan-revenue-analysis.git cd telecom-plan-revenue-analysis ``` 
   
   2. **(Optional) Create and activate a virtual environment:** 
   
   ```bash python3 -m venv venv source venv/bin/activate # macOS/Linux venv\Scripts\activate # Windows ``` 
   
   3. **Install dependencies:** 
   
   ```bash pip install -r requirements.txt ``` 
   
   4. **Launch Jupyter Notebook:** 
   
   ```bash jupyter notebook ``` 
   
   5. **Open `analysis.ipynb`** and run all cells to explore the analysis. </pre>
