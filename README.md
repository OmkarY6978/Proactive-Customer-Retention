Customer Segmentation & Churn Prediction
<p align="center">
<a href="https://www.python.org" target="_blank">
<img src="https://img.shields.io/badge/Python-3.9+-blue.svg" alt="Python version">
</a>
<a href="https://scikit-learn.org/" target="_blank">
<img src="https://img.shields.io/badge/Framework-Scikit--learn-orange" alt="Scikit-learn">
</a>
<a href="https://vercel.com" target="_blank">
<img src="https://img.shields.io/badge/Deployment-Vercel-black" alt="Vercel">
</a>
</p>

This project analyzes customer transaction data to build a proactive retention strategy. It segments customers using RFM analysis and K-Means clustering, then predicts churn risk with a Random Forest model. The final result is an interactive dashboard for business users to explore customer segments and view recommended marketing actions.

🚀 Live Demo & Screenshots
You can view the live interactive dashboard deployed on Vercel:

[Live Demo Link Here] 👈 (Replace this with your actual Vercel link)

<br>

<p align="center">
(Optional: Add a screenshot of your dashboard here for a great first impression!)
<br>
![Dashboard Screenshot](link_to_your_screenshot.png)
</p>

🎯 Project Goal
The core objective is to leverage data science to reduce customer churn. By understanding different customer personas and their behavior, the business can move from generic marketing to targeted, personalized strategies that enhance customer loyalty and lifetime value.

🛠️ Our Methodology
The project follows a structured data science workflow:

Data Cleaning & Preparation: Loaded raw transactional data, handled missing values (especially Customer ID), and removed inconsistencies like return transactions.

Feature Engineering (RFM Analysis): Calculated Recency, Frequency, and Monetary (RFM) scores for each customer to create a powerful behavioral profile.

Customer Segmentation (K-Means Clustering): Applied K-Means clustering to group customers into 4 distinct segments. These segments were analyzed and given meaningful labels.

Churn Prediction (Random Forest): Defined "churn" as customer inactivity for over 90 days and trained a RandomForestClassifier to predict this outcome, focusing on high Recall to catch as many at-risk customers as possible.

Actionable Visualization: Developed an interactive HTML dashboard to present the findings, allowing business users to easily filter and explore the data.

📊 Key Findings & Business Strategies
Our analysis provides a clear framework for targeted marketing:

Segment

Characteristics

Recommended Strategy

🏆 Champions

High spenders, frequent, and recent buyers.

Reward with loyalty programs, exclusive access, and personalized thank yous.

⭐ Potential Loyalists

Consistent customers with room for growth.

Nurture with targeted promotions, cross-sell related products, and build engagement.

🌱 New Customers

Made their first few purchases recently.

Focus on a smooth onboarding experience and offer first-time purchase discounts.

⚠️ At-Risk

Haven't purchased in a long time; high churn risk.

IMMEDIATE ACTION: Launch personalized win-back campaigns with special discounts.

⚙️ Technology Stack
Language: Python 3

Libraries: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

Frontend: HTML5, CSS (with Tailwind CSS), JavaScript

Deployment: Vercel

🚀 How to Run This Project Locally
To get a local copy up and running, follow these simple steps.

Prerequisites
Make sure you have Python 3 installed on your system.

1. Clone the Repository
git clone https://github.com/YOUR_USERNAME/customer-dashboard.git
cd customer-dashboard

2. Install Dependencies
Install the required Python libraries using pip:

pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab

3. Run the Analysis
Place the online_retail_II.csv file (downloaded from Kaggle) in the root of the project directory.

Run the Jupyter Notebook (.ipynb file) to execute the analysis and generate the customer_action_plan.csv file.

4. Generate JSON Data for the Dashboard
Run the conversion script from your terminal:

python convert_to_json.py

5. View the Dashboard
Open the index.html file in your web browser to see the interactive dashboard.
