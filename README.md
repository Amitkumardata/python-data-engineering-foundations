🛒 Customer Lifetime Value Prediction & RFM Segmentation invoice accross 37 countries) we apply RFM behavirff
End-to-End Data Analytics Capstone | E-commerce · ML · Business Intelligence
Python
Zoom
Download
 Status
Zoom
 
Download
 License
Zoom

Download
 Pandas


📌 Business Problem
The marketing and customer succcess team at a UK-based online retailer needs to Idenitfy high- value customers
segments and predict 12 month customer lifetime value (LTV) in order to preotize retention spend and personalize re-engagement compaigns

Currently, all customers receive the same discount offers regardless of thier value tier, resulting in wasted budget on low LTV customers and under investment in the top 20% who drive 
approxematly 65% of revnenue

Using 2+ years of transactional data ( 541,910 invoice accross 37 countries) 
we apply RFM behavioral segmentation and a predictive LTV model to produce a customer -level scoring table and an Intractive plotly dashboard that a non-Technical stakeholder can act on Immediately 

🎯 Success Metrics

Metric	    Target	      Why It Matters
LTV Model R²	   ≥ 0.75	     Explains 75%+ of LTV variance
RMSE (normalized)    	≤ 15%	        Prediction error acceptable for budget planning
RFM Segment Separation	    p < 0.05 (ANOVA)	    Segments are statistically distinct
Pareto Validation	       Top 20% customers ≥ 60% revenue	     Confirms business assumption
Dashboard Usability       	Non-technical stakeholder can filter & interpret      	Business impact validated

🗃️ Dataset
Source: Online retailer -- UCI Maachine Learning repository 
Alos on kaggle: Mashlyn/online -retail 11 uci
time-period: DEC 2009 - DEC 2011
Size -1,000,000 rows * 8 columns 

# Schema

Column      type       Description
Invoice     string     unique Transaction ID(Prefix 'C' =Cancellation)
StockCode   String    Product/Item Code 
Description  String   Product Name 
Quanity       INT      unit purchased 
Invoice Date   Datetime  Transaction  Timestamp
Price          Float   Unit price in GBP
CustomerID     fLOAT   Unique customer Identity 
Country      String    Customer country 

🗺️ Project Roadmap
week 1 : END- TO END Execution
DAY 1 Project scoping & data discovery 
DAY 2 Exploratory Data analysis (EDA)
Day 3 Data cleaning & Feature Engineering 
Day 4 Statistical Analysis & Hypothesis Testing
Day 5 ML Modeling LTV Prediction 
DAY 6 Visualization & story telling (Plotly Dashboard)
Day 7 GitHub Polish & Portfolio Presentation

🏗️ Project Structure
 

capstone-ecommerce-ltv/
│
├── data/
│   ├── raw/                    # Original unmodified data (not committed)
│   ├── processed/              # Cleaned, feature-engineered data
│   └── external/               # Reference data (e.g., country codes)
│
├── notebooks/
│   ├── 01_data_discovery.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_cleaning_features.ipynb
│   ├── 04_statistical_analysis.ipynb
│   ├── 05_ltv_model.ipynb
│   └── 06_dashboard.ipynb
│
├── src/
│   ├── data/           load_data.py, validate_schema.py
│   ├── features/       rfm_calculator.py, ltv_features.py
│   ├── models/         train.py, evaluate.py, predict.py
│   └── visualization/  plots.py, dashboard.py
│
├── outputs/
│   ├── figures/        All exported charts (.html, .png)
│   ├── models/         Saved model artifacts (.pkl)
│   └── reports/        Final analysis reports
│
├── docs/
│   ├── problem_statement.md
│   ├── data_dictionary.md
│   └── methodology.md
│
├── tests/              Unit tests for src/ modules
├── requirements.txt
├── .gitignore
└── README.md
🔬 Methodol

🔬 Methodology

Phase 1 — RFM Segmentation

* Compute Recency , Frequence, Monetory per customer
* Score each dimension(1-5 quitiles)
* Assign behavioral segment chapions , loyal , At-Rish , Lost
* Validate with ANOVA across segment revenue distributions

 Phase 2 — LTV Prediction

 * Feature Engineering: Purchase Cadence , AOV, Product Diversity, Seasonality
 * Target: Total Revenue in next 12 month(Regression problem)
 * Model: XGboost Regression with cross validation
 * Explainability: Shap values for feature Importance
 * Evaluation: R2 , RMSE , MAE On holdout set

Phase 3 — Business Dashboard

* Interactive & Dynamic Dashboard or HTML Dashbaord
* Filters: Segment , country, data range
* Outputs: Customers scoring table, revenue concentration chart, RFM Heatmap
  

   








