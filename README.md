## 📘 Business Owners Insights Dashboard

An end-to-end data analytics project analyzing 104,000+ Indian businesses using Power BI, SQL, and Python, uncovering trends in business distribution, ownership patterns, and regional insights.

🖥️ Dashboard Preview

⭐ 1. Business Overview Dashboard
<img width="1279" src="https://github.com/user-attachments/assets/8414315e-8f95-44f4-b06d-d3034c53496b" />
⭐ 2. Owner Insights Dashboard
<img width="1278" src="https://github.com/user-attachments/assets/30fa0257-d9f0-4433-8c0f-7c8749703761" />
⭐ 3. City-Level Analysis Dashboard
<img width="1281" src="https://github.com/user-attachments/assets/5f5606fa-2d55-486d-87a0-4980e0629292" />
⭐ 4. Business Overview Heatmap
<img width="1267" src="https://github.com/user-attachments/assets/06933646-238c-45fd-979a-e74b745dd2db" />
🎯 Objectives

Clean & standardize 100K+ business records

Fix inconsistent state & city naming

Build business_category using Python NLP

Develop four Power BI dashboards

Generate insights for business strategy & planning

🛠 Tech Stack
Category	Tools
🗄️ Database	MySQL
🐍 Programming	Python (Pandas, Regex)
📊 BI Tool	Power BI
☁️ Notebook	Google Colab
📂 Dataset Fields

business_name

owner_name

city

state

mobile_number

business_category (engineered with Python NLP)

🧹 Data Cleaning (SQL)

Removed duplicates

Normalized states (36 cleaned values)

Standardized city names

Validated and handled missing values

SELECT state, COUNT(*) 
FROM business_owners
GROUP BY state
ORDER BY COUNT(*) DESC;

🤖 Business Categorization (Python NLP)
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


Produces 10 final business categories.

📈 Key Insights

Maharashtra ranks #1 with 21K+ businesses

IT / Software is the fastest-growing category (26K+ businesses)

Retail / Trading has the widest geographic spread

8,331 owners operate multiple businesses

One owner controls 147 businesses

Top cities: Mumbai, Chennai, Delhi, Ahmedabad, Pune

📦 Deliverables

✔ Clean SQL dataset

✔ Python categorization script

✔ Power BI .pbix file

✔ Dashboard screenshots

✔ Insights summary

✔ Complete GitHub documentation

👤 About the Author

Shekhar Suman
Aspiring Data Analyst
Power BI • SQL • Python • Data Visualization
