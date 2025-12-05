Power BI • SQL • Python (NLP) • Data Analytics Project
📝 Project Overview

This project analyzes a large real-world dataset of 100,000+ Indian business owners.
The goal was to transform raw, unstructured data into meaningful business intelligence dashboards by using:

MySQL for data cleaning

Python (NLP) for business categorization

Power BI for interactive dashboards

The final solution helps identify:

Business distribution across states and cities

Industry trends

Multi-business owners

Regional strengths across India

🎯 Objectives

✔ Clean & transform raw dataset (100K+ records)
✔ Standardize inconsistent state/city names
✔ Engineer new insights using NLP-based business classification
✔ Build 4 professional Power BI dashboards
✔ Provide actionable insights for business and market analysis

🛠 Tech Stack
Category	Tools
Database	MySQL (Workbench)
Programming	Python, Pandas
ML/NLP	Keyword-based classification
Visualization	Power BI Desktop
Environment	Google Colab
📂 Dataset Fields

business_name

owner_name

city

state

mobile_number

After NLP enrichment:

business_category (10 categories)

🧹 Phase 1 — Data Cleaning (SQL)

Performed:

Removal of duplicates

Fixing inconsistent state names

Standardizing city formatting

Checking null/missing values

Exporting clean dataset

Example SQL used:

SELECT state, COUNT(*) 
FROM business_owners 
GROUP BY state 
ORDER BY COUNT(*) DESC;

🤖 Phase 2 — NLP-Based Business Categorization (Python)

Since the dataset had no business industry,
I built a Python NLP function to classify businesses into:

IT / Software

Retail / Trading

Construction / Real Estate

Interior / Decor

Consulting

Fashion / Textile

Transport / Logistics

Finance

Education

Other

Python snippet:

def categorize_business(name):
    name = str(name).lower()
    if any(x in name for x in ['tech','software','it','solutions']):
        return 'IT / Software'
    elif any(x in name for x in ['shop','store','trading']):
        return 'Retail / Trading'
    elif any(x in name for x in ['construction','infra','builders']):
        return 'Construction / Real Estate'
    elif any(x in name for x in ['fashion','textile','boutique']):
        return 'Fashion / Textile'
    else:
        return 'Other'

📊 Phase 3 — Power BI Dashboard

The project includes four interconnected dashboards:

🖼 📌 Dashboard Screenshots

⚠️ IMPORTANT:
Replace the image links below with your GitHub image URLs after uploading.

⭐ 1. Business Overview Dashboard
<img src="https://raw.githubusercontent.com/your_username/your_repo/main/overview.png" width="900">
⭐ 2. State vs Business Category Heatmap
<img src="https://raw.githubusercontent.com/your_username/your_repo/main/state_heatmap.png" width="900">
⭐ 3. City Level Analysis
<img src="https://raw.githubusercontent.com/your_username/your_repo/main/city_analysis.png" width="900">
⭐ 4. Owner Insights Dashboard
<img src="https://raw.githubusercontent.com/your_username/your_repo/main/owner_insights.png" width="900">
📈 Key Insights
🔹 1. Maharashtra is India's Business Capital

Most businesses

Leader in IT, Retail & Real Estate

Mumbai alone contributes the highest across multiple categories

🔹 2. IT / Software is the largest identified industry

26,739 IT-related businesses

Strong in Maharashtra, Karnataka, Tamil Nadu, Telangana

🔹 3. Retail / Trading is widespread across India

Appears in almost all states and major cities.

🔹 4. Multi-Business Ownership is Common

One owner has 147 businesses

Several owners hold 100+ businesses

Maharashtra & Gujarat have the highest multi-business owners

🔹 5. City-Level Trends

Mumbai → IT + Retail dominant

Chennai → IT + Services

Ahmedabad → Retail + Trade heavy

Delhi → Mixed business categories

📁 Project Deliverables

✔ Cleaned dataset (business_owners_final.csv)
✔ Python notebook for NLP classification
✔ Power BI dashboard (.pbix file)
✔ Insight summary & visualizations
✔ GitHub project documentation

🏁 Conclusion

This project demonstrates end-to-end data analytics capability, covering:

Data cleaning

Feature engineering

NLP-based enrichment

Insights extraction

BI dashboard design

It provides a clear view of India's business landscape and reveals patterns in state, city, and owner-level distributions.

🙋‍♂️ Author

Shekhar Suman
Aspiring Data Analyst | Power BI | SQL | Python | BI Dashboards
