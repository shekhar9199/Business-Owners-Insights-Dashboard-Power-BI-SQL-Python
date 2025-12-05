📘 Business Owners Insights Dashboard
Power BI • SQL • Python • Data Analytics Project
📝 Project Overview

This project analyzes a real-world dataset of 104,000+ Indian businesses to uncover insights related to:

Business distribution across states and cities

Owner-level business concentration

Industry category segmentation

Regional business patterns

The solution demonstrates end-to-end Data Analytics & BI development using SQL, Python, and Power BI.

🎯 Objectives

✔ Clean and standardize 100K+ raw records
✔ Fix inconsistent state & city names
✔ Create automated business category classification using Python (NLP)
✔ Build four professional Power BI dashboards
✔ Generate insights useful for business planning & market analysis

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

New Feature Engineered (Python NLP)

business_category (10 categories extracted from business_name)

🧹 Phase 1 — Data Cleaning (SQL)

Performed:

Duplicate removal

State name normalization (36 unique states after cleaning)

City formatting standardization

Validation of missing values

Export of cleaned dataset

Example Query

SELECT state, COUNT(*) 
FROM business_owners 
GROUP BY state
ORDER BY COUNT(*) DESC;

🤖 Phase 2 — Business Categorization (Python NLP)

Business names were classified into industry sectors using keyword matching.

Example:

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


This produced 10 business categories, including IT, Retail, Consulting, etc.

📊 Phase 3 — Power BI Dashboards

A complete BI solution with four interconnected dashboards was built.

🖼 📌 DASHBOARD SCREENSHOTS

⚠️ Replace the image URLs with your real GitHub links after uploading.

⭐ 1. Business Overview Dashboard
<img width="1279" height="707" alt="Image" src="https://github.com/user-attachments/assets/8414315e-8f95-44f4-b06d-d3034c53496b" />
⭐ 2. Owner Insights Dashboard
<img width="1278" height="719" alt="Image" src="https://github.com/user-attachments/assets/30fa0257-d9f0-4433-8c0f-7c8749703761" />
⭐ 3. City-Level Analysis Dashboard
<img width="1281" height="717" alt="Image" src="https://github.com/user-attachments/assets/5f5606fa-2d55-486d-87a0-4980e0629292" />
⭐ 4. Business Overview Heatmap
<img width="1267" height="715" alt="Image" src="https://github.com/user-attachments/assets/06933646-238c-45fd-979a-e74b745dd2db" />
📈 Key Insights Extracted
🔹 1. Maharashtra Dominates Indian Business Landscape

21K+ businesses

Leads in IT, Retail, Construction

🔹 2. IT / Software is the Fastest-Growing Category

26K+ businesses

Highly concentrated in:

Bangalore

Chennai

Hyderabad

Mumbai

🔹 3. Retail / Trading is the Most Widely Spread Category

Appears across all states and nearly every city.

🔹 4. Multi-Business Ownership is Significant

8,331 owners have more than 1 business

One owner holds 147 businesses

Gujarat & Maharashtra have the highest multi-business ownership concentration

🔹 5. Top Business Cities

Mumbai

Chennai

Delhi

Ahmedabad

Pune

📁 Project Deliverables

✔ Clean SQL-transformed dataset
✔ Python classification script
✔ Final Power BI .pbix dashboard
✔ Insights summary
✔ GitHub documentation (this README)

🧑‍💼 About the Author

Shekhar Suman
Aspiring Data Analyst
Power BI | SQL | Python | Data Visualization
