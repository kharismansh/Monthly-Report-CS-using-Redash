# 📊 Monthly CS Reporting Automation (Redash)

This repository contains a Python-based notebook (Google Colab / Jupyter) designed to automate monthly reporting for CS by extracting data from Redash, processing it, and distributing reports via email.

---

# 📌 Business Background

Stakeholder requires clear visibility to monitor monthly performance.
In this project, the monthly CS report is defined as a report that displays all order activities for each shipper within a given month.

This report enables the stakeholder to:
- Track the status of all orders within the reporting period
- Provide structured and consistent information to each shipper
- Improve monitoring and decision-making based on monthly performance
  
# 🚀 Overview

This project automates the end-to-end reporting process:
- Retrieve data from Redash
- Process and clean raw data using Python
- Generate summary reports per shipper
- Send automated email reports to stakeholders

---

# 🛠️ Tech Stack
- Python
- Pandas
- Requests (API integration)
- SMTP (email automation)
- Google Colab / Jupyter Notebook
- Redash as data source

---

# ⚙️ How It Works
1. Define Reporting Period
2. Configure Shipper List
3. Fetch Data from Redash (Call Redash API, Retrieve data using a specific query ID, Store results in a Pandas DataFrame)
4. Data Processing, Includes:
   - Selecting relevant columns
   - Handling missing values
   - Grouping data by shipper
   - Identifying inactive shippers (no orders)
5. Generate Reports
   - Data is grouped per shipper
   - Pivot tables are created for summary reporting
   - Output is prepared for distribution
6. Send Emails, the system will send reports individually per shipper, sutomatically generate subject lines based on the reporting period and attach detailed report files

---

# 📧 Output

Each stakeholder will receive:
- Monthly Corporate Sales report
- Summary of order performance (pivot table)
- Attached file containing detailed data
- Easy-to-access and downloadable reports via email

---

# 📊 Impact
- Reduced manual reporting effort through automation
- Improved reporting consistency and accuracy
- Enabled faster and more informed decision-making
- Provided clear visibility of monthly performance per shipper

---

# 🔐 Notes
- Ensure Redash API access is properly configured (API Key / Query ID)
- Do not expose sensitive credentials (email, password, API keys) in the repository
- Use environment variables for better security

---

## 🙋‍♀️ Author

Kharisma Nur’aisyah  
[LinkedIn](https://www.linkedin.com/in/kharismanuraisyah/)
