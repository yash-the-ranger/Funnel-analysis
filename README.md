📌 Project Overview

This project analyzes an end-to-end e-commerce conversion funnel to identify user drop-offs, quantify conversion efficiency at each stage, and provide data-driven business recommendations. The analysis combines SQL, Python (Matplotlib & Plotly), and Power BI to deliver both analytical depth and executive-ready visualizations.

The funnel tracks users across the following stages:
Visit → View Product → Add to Cart → Checkout → Purchase

🎯 Business Objectives

Understand where and why users drop off in the purchase journey

Measure stage-wise and overall conversion rates

Identify high-impact optimization areas (especially near checkout)

Support decisions with clear visual evidence and SQL-backed metrics

🗂️ Dataset Description

The dataset represents user interaction events captured from an e-commerce platform.

Key fields:

user_id – unique user identifier

event_type – funnel stage (visit, view_product, add_to_cart, checkout, purchase)

event_time – timestamp of the event

device – desktop / mobile / tablet

traffic_source – marketing acquisition source

🧠 Key Insights

Conversion declines steadily across the funnel, indicating increasing friction closer to purchase.

The largest drop-off occurs between checkout and purchase, highlighting last-step friction.

Early-stage engagement is relatively healthy; optimization efforts should prioritize checkout completion, not traffic volume.

Device segmentation (via SQL) enables prioritization of mobile-first improvements.

💡 Business Recommendations

Simplify checkout flow (reduce form fields, enable autofill).

Surface shipping cost, taxes, and delivery ETA earlier.

Improve payment reliability with retries and clearer failure handling.

Optimize checkout UX for mobile devices (tap targets, performance, validation).

Perform focused QA on mobile browsers (Android Chrome, iOS Safari).

📊 Visualizations

The project includes visual analysis using both BI tools and Python libraries.

Power BI Dashboard

KPI cards (Overall Conversion, Visit Users, Purchase Users)

Funnel overview with user drop-offs

Stage conversion performance table

Conversion trend visualization

Device slicer for segmentation

Python Visualizations

Matplotlib (static, report-ready):

Funnel drop-off bar chart

Stage-wise conversion trend line

Plotly (interactive):

Device-wise conversion comparison

Sankey diagram showing user flow across stages

🧾 SQL Analysis

All metrics are backed by SQL queries written in MySQL 8+, including:

Distinct user counts per funnel stage

Stage-to-stage conversion and drop-off rates

Overall conversion rate

Device-wise conversion using a one-device-per-user rule

Each SQL query is documented with:

Business question

Expected analytical outcome

Query logic

🛠️ Tools & Technologies

Power BI – Dashboarding & business reporting

SQL (MySQL 8+) – Funnel metrics & aggregation

Python

Pandas – data preparation

Matplotlib – static visualizations

Plotly – interactive charts

Excel – exploratory checks & validation



📂 Project Structure

├── powerbi/
│   └── funnel_analysis_dashboard.pbix
├── sql/
│   └── funnel_analysis_queries.sql
├── python/
│   ├── funnel_visualizations.py
│   └── device_analysis.py
├── report/
│   └── Funnel_Analysis_Report.pdf
└── README.md

🚀 How to Run

Execute SQL scripts to compute funnel metrics.

Load aggregated results into Power BI for dashboarding.

Run Python scripts to generate Matplotlib and Plotly visuals.

Review insights and recommendations in the final report.

📈 Outcome

This project demonstrates the ability to:

Translate raw event data into actionable business insights

Combine SQL, Python, and BI tools in a single workflow

Communicate findings clearly to both technical and non-technical stakeholders
