.

📘 Business Owners Insights Dashboard
Power BI • SQL • Python • Data Analytics Project

A complete end-to-end analytics project built using SQL, Python, and Power BI, analyzing 104,000+ Indian business records to uncover patterns in business distribution, ownership behavior, and regional trends.

📝 Project Overview

This project provides a full data analytics workflow:

Cleaning and preparing raw business-owner data

Categorizing business names using Python NLP

Performing SQL-based exploration

Designing four professional Power BI dashboards

Extracting insights useful for business strategy, market research & regional planning

🎯 Key Objectives

✔ Clean and standardize 100K+ business records
✔ Fix inconsistent state/city names
✔ Engineer business category using Python (keyword-based NLP)
✔ Build interactive dashboards in Power BI
✔ Identify state, city & owner-level business patterns
✔ Produce actionable insights for decision-making

🛠 Tech Stack
Category	Tools
Database	MySQL
Programming	Python (Pandas, Regex)
Business Intelligence	Power BI
Cloud Notebook	Google Colab
📂 Dataset Fields

business_name

owner_name

city

state

mobile_number

🔧 Feature Engineered (Python NLP)

business_category → 10 new categories generated from business_name

🧹 Phase 1 — Data Cleaning (SQL)

Performed:

Removal of duplicate & invalid entries

Standardization of 36 unique state names

City name normalization

Validation of missing values

Export of cleaned dataset

✔ Example Query

SELECT state, COUNT(*) 
FROM business_owners 
GROUP BY state
ORDER BY COUNT(*) DESC;

🤖 Phase 2 — Business Categorization (Python NLP)

A rule-based NLP classifier was created to identify industry sectors from business names.

def categorize_business(name):
    name = str(name).lower()
    if any(x in name for x in ['tech','software','solutions']):
        return 'IT / Software'
    elif any(x in name for x in ['shop','trading','retail']):
        return 'Retail / Trading'
    elif any(x in name for x in ['infra','builders','construction']):
        return 'Construction / Real Estate'
    else:
        return 'Other'


🔹 Result: 10 consistent categories such as IT, Retail, Consulting, Construction, etc.

📊 Phase 3 — Power BI Dashboards

A complete BI solution with four interactive dashboards.

🖼 Dashboard Screenshots

(Images already updated — GitHub will render them automatically)

⭐ 1. Business Overview Dashboard
<img width="1279" src="https://github.com/user-attachments/assets/8414315e-8f95-44f4-b06d-d3034c53496b" />
⭐ 2. Owner Insights Dashboard
<img width="1278" src="https://github.com/user-attachments/assets/30fa0257-d9f0-4433-8c0f-7c8749703761" />
⭐ 3. City-Level Analysis Dashboard
<img width="1281" src="https://github.com/user-attachments/assets/5f5606fa-2d55-486d-87a0-4980e0629292" />
⭐ 4. Business Overview Heatmap
<img width="1267" src="https://github.com/user-attachments/assets/06933646-238c-45fd-979a-e74b745dd2db" />
📈 Key Insights Extracted
🔹 1. Maharashtra leads Indian business growth

21K+ businesses

Strong presence in IT, Retail, Construction

🔹 2. IT / Software dominates high-growth sectors

26K+ businesses

Highly concentrated in Bangalore, Chennai, Hyderabad, Mumbai

🔹 3. Retail / Trading is the most widely distributed

Present in nearly every Indian city

🔹 4. Multi-business ownership is significant

8,331 owners have multiple businesses

One owner operates 147 businesses

Highest concentration in Gujarat & Maharashtra

🔹 5. Top Business Cities

Mumbai

Chennai

Delhi

Ahmedabad

Pune

📁 Project Deliverables

✔ Clean SQL-transformed dataset
✔ Python business-category script
✔ Power BI .pbix interactive dashboards
✔ Insights summary
✔ Complete GitHub documentation (this README)

👤 About the Author

Shekhar Suman
Aspiring Data Analyst
Power BI | SQL | Python | Data Visualization

💼 Open to Data Analyst / BI Analyst roles
📧 Email: (add your email here)
🔗 LinkedIn: (add your LinkedIn link)
