Customer Retention & Churn Analysis Dashboard
<p align="center">
<strong>A data-driven approach to understanding and retaining valuable customers for an online retailer.</strong>
</p>

<p align="center">
<a href="#-live-demo">View Live Demo</a> •
<a href="#-project-goal">Project Goal</a> •
<a href="#-our-process">Our Process</a> •
<a href="#-technology-stack">Tech Stack</a> •
<a href="#-running-locally">Running Locally</a>
</p>

<p align="center">
<img src="https://i.imgur.com/g9vD2mJ.png" alt="Dashboard Screenshot" width="80%">
<em>(An interactive dashboard built to turn complex data into actionable insights.)</em>
</p>

🤔 The Problem: Why Do Customers Leave?
For any online retailer, customer acquisition is expensive. The real challenge lies in customer retention. This project tackles a critical business question: Can we identify customers who are about to leave before they do? Relying on guesswork leads to wasted marketing budget and lost revenue. We need a way to pinpoint at-risk customers and understand our most loyal ones to act effectively.

✨ Our Solution: A Proactive Strategy
This project moves beyond simple sales reporting to build a proactive retention engine. By analyzing over a year of transactional data, we developed a system that:

Segments customers into meaningful groups based on their purchasing behavior.

Predicts churn risk using a machine learning model.

Provides clear, actionable recommendations through an interactive dashboard designed for business decision-makers.

🗺️ Our Process: From Raw Data to Actionable Insights
Our workflow was structured to ensure a robust and meaningful outcome.

<p align="center">
<code>Data Cleaning</code> ➔ <code>RFM Analysis</code> ➔ <code>K-Means Clustering</code> ➔ <code>Churn Modeling</code> ➔ <code>Interactive Dashboard</code>
</p>

Data Cleaning & Preparation: The initial dataset was noisy. We handled missing values, removed return transactions, and structured the data for analysis.

RFM Feature Engineering: We created a customer DNA using RFM scores:

R (Recency): How recent was their last purchase?

F (Frequency): How often do they buy?

M (Monetary): How much do they spend?

Unsupervised Clustering: Using K-Means, we let the data speak for itself, revealing 4 distinct customer personas.

Predictive Modeling: We trained a Random Forest model to predict which customers were likely to churn, allowing the business to intervene preemptively.

👥 Customer Personas Uncovered
Our analysis identified four key customer segments, each with its own unique characteristics and required strategy.

Persona

Key Characteristics

Recommended Action

🏆 Champions

Your most valuable and loyal customers. They buy often and spend the most.

Reward them. Offer exclusive access, loyalty points, and personalized engagement.

⭐ Potential Loyalists

Consistent customers who show potential to become Champions.

Nurture them. Use targeted marketing and cross-selling to increase their frequency and spend.

🌱 Newcomers

First-time or very recent buyers. The crucial first impression phase.

Onboard them. Provide a great initial experience and incentives for a second purchase.

⚠️ At-Risk

Customers who haven't purchased in a long time. High risk of leaving.

Re-engage them. Launch targeted "we miss you" campaigns with compelling offers to win them back.

⚙️ Technology Stack
This project was built using a combination of data science and web development tools.

Backend & Analysis: Python, Pandas, NumPy, Scikit-learn

Data Visualization: Matplotlib, Seaborn

Frontend Dashboard: HTML5, Tailwind CSS, JavaScript

Deployment: Vercel

🚀 Running Locally
Want to explore the project on your own machine? Follow these steps.

1. Clone the Repository
git clone https://github.com/YOUR_USERNAME/customer-dashboard.git
cd customer-dashboard

(Replace YOUR_USERNAME with your actual GitHub username)

2. Install Dependencies
pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab

3. Run the Analysis & Prepare Data
Download the dataset from Kaggle and place online_retail_II.csv in the project folder.

Run the Jupyter Notebook to generate the customer_action_plan.csv.

Run the conversion script to create the dashboard's data source:

python convert_to_json.py

4. View the Dashboard
Simply open the index.html file in your browser to see the final result.

<p align="center">
<em>This project was created as a demonstration of a full-stack data science workflow, from data analysis to a user-facing product.</em>
</p>
