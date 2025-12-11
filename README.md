# Customer_Behavior_Analysis
Data analytics project showcasing customer behavior analysis using Python, SQL, Power Bi

🛍️ Customer Shopping Behavior AnalysisProject OverviewThis data analysis project investigates the shopping patterns of a retail company's customer base to uncover key business insights. 
The goal is to provide data-driven recommendations for improving sales, optimizing marketing strategies, and enhancing customer retention.

Problem: A retail company is facing changing purchasing patterns and needs to understand which factors (e.g., discounts, reviews, subscription status, shipping type) significantly influence consumer spending and behavior.

💾 Dataset DetailsThe analysis is based on a customer shopping behavior dataset.
MetricDetailSourceProvided retail company dataRecords (Rows)3,900Features (Columns)18 (e.g., Gender, Item Purchased, Purchase Amount (USD), Review Rating)

🛠️ Tools and Technologies:-
CategoryTools
UsedPurposeData PreparationPython (Pandas)Cleaning, 
feature engineering, and exploratory data analysis (EDA).
Database ManagementPostgreSQLData warehousing and executing complex analytical SQL queries.
AnalysisSQLDeep-dive analysis to answer key business questions and extract insights.

VisualizationPower BICreating an interactive dashboard for visual reporting and stakeholder communication.

PresentationGammaDeveloping the final project presentation (PPT).

Version ControlGitHubProject documentation and version tracking.

🚀 Project Steps & Methodology

The project followed a standard data science lifecycle:

1. Exploratory Data Analysis (EDA) & CleaningData Cleaning: Handled data inconsistencies, checked for duplicates, and ensured data types were correct.Imputation: Missing values in the Review Rating column were filled using the median rating for each product category for a more accurate representation.Feature Engineering: Created new derived features, such as Age Group (e.g., Young Adult, Middle-Aged) and mapped purchase frequency strings to numerical values for quantitative analysis.

2. Database Loading and SQL AnalysisThe cleaned data was loaded into a PostgreSQL table named customer.Complex SQL queries were executed to answer specific business questions (e.g., "Do subscribed customers spend more?" and "Which customers use discounts but still have high spending?").

3. Key SQL InsightsRevenue Split: Revenue is nearly equally split between male and female customers, requiring targeted campaigns for both.High-Value Discount Users: Identified a critical segment of 784 customers who use discounts but still spend above the average, indicating discounts act as a final purchase incentive for large transactions.Shipping Preference: Customers who choose Express Shipping have a slightly higher Average Purchase Amount (AOV), suggesting they value speed and are willing to spend more.Subscription Effectiveness: Non-subscribed customers currently have a slightly higher average spend than subscribed customers.

4. Power BI Dashboard DevelopmentAn interactive dashboard was created to visualize KPIs (Total Revenue, AOV, Avg. Rating) and trend analysis (Revenue by Category, Age Group).The dashboard allows stakeholders to filter and drill down by Gender, Subscription Status, and Shipping Type.

🎯 Results and Business Recommendations:-

The analysis yielded actionable recommendations focused on improving profitability and customer engagement:Subscription Revamp: Revise the subscription program to include tiered benefits or exclusive access to premium products to drive a higher Average Order Value (AOV) for subscribers.Targeted Discount Strategy: Create a loyalty track for the identified high-value discount users, rewarding them with special, personalized promotions on premium items to maintain their high spending.Invest in Express Shipping: Actively promote Express Shipping, potentially offering it free above a higher order threshold, as it is correlated with higher-spending customers.Leverage High-Rated Products: Feature the top-rated products (e.g., Gloves, Sandals, Boots) prominently in marketing as a testament to brand quality.⚙️ How to Run the Project LocallyTo replicate the analysis, follow these steps:Clone the Repository:Bashgit clone.
cd customer-shopping-behavior-analysis

Database Setup:Install and run PostgreSQL.Create a database named customer_behavior.Run Python Analysis:Open and execute the customer_behaivor_analysis.ipynb file (which includes feature engineering and connecting to PostgreSQL to load the data).Note: Update the database connection credentials in the notebook.View Dashboard:Download and install Power BI Desktop.Open the customer_behavior.pbix file to explore the interactive dashboard.
