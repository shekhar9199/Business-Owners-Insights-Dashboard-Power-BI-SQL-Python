📘 <h1 align="center">Business Owners Insights Dashboard</h1>
<p align="center"> End-to-end analytics project analyzing <strong>104,000+ Indian businesses</strong> using Power BI, SQL & Python. Reveals insights on business distribution, ownership patterns & regional trends across India. </p>
<br>
<h1>🖼️ Dashboard Preview</h1>
<br>
⭐ 1. Business Overview
<p align="center"><img width="800" src="https://github.com/user-attachments/assets/8414315e-8f95-44f4-b06d-d3034c53496b" /></p> <br>
⭐ 2. Owner Insights
<p align="center"><img width="800" src="https://github.com/user-attachments/assets/30fa0257-d9f0-4433-8c0f-7c8749703761" /></p> <br>
⭐ 3. City-Level Analysis
<p align="center"><img width="800" src="https://github.com/user-attachments/assets/5f5606fa-2d55-486d-87a0-4980e0629292" /></p> <br>
⭐ 4. Business Heatmap
<p align="center"><img width="800" src="https://github.com/user-attachments/assets/06933646-238c-45fd-979a-e74b745dd2db" /></p>
<br>

<h2>🎯 Objectives</h2>
<br>

Clean & standardize 100K+ business records

Fix inconsistent state & city names

Build business categories using Python NLP

Design four Power BI dashboards

Provide actionable insights for business strategy

<br>
🛠 Tech Stack
🔥 Premium Card Layout
<br> <table> <tr> <td width="250"><strong>🗄️ Database</strong><br>MySQL</td> <td width="250"><strong>🐍 Programming</strong><br>Python (Pandas, Regex)</td> </tr> <tr> <td><strong>📊 BI Tool</strong><br>Power BI</td> <td><strong>☁️ Notebook</strong><br>Google Colab</td> </tr> </table>
<br>
📂 Dataset Fields
<br>
business_name
owner_name
city
state
mobile_number
business_category  (engineered with Python NLP)

<br>
🧹 Data Cleaning (SQL)
<br>

Performed:

✔ Duplicate removal
✔ State normalization (36 consistent names)
✔ City standardization
✔ Missing value handling

<br>
SELECT state, COUNT(*) 
FROM business_owners
GROUP BY state
ORDER BY COUNT(*) DESC;

<br>
🤖 Business Categorization (Python NLP)
<br>
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


✔ Categorizes records into 10 final business groups

<br>
<h2>📈 Key Insights</h2>
<br>

Maharashtra leads with 21K+ businesses

IT / Software is fastest-growing with 26K+ firms

Retail/Trading shows widest presence across India

8,331 owners run multiple companies

One owner manages 147 businesses

Top cities: Mumbai, Chennai, Delhi, Ahmedabad, Pune

<br>
📦 Deliverables
<br>

✔ Cleaned SQL dataset
✔ Python NLP categorization script
✔ Power BI .pbix report
✔ Dashboard screenshots
✔ Insight summary
✔ Polished documentation

<br>
👤 About the Author
<br>

Shekhar Suman
Aspiring Data Analyst
Specializing in Power BI • SQL • Python • Visualization

<br> <p align="center"> Made with ❤️ for data analytics & real-world insights. </p>
