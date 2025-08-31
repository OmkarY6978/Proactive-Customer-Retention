# Customer Retention & Churn Analysis Dashboard

<p align="center">
  <strong>A data-driven approach to understanding and retaining valuable customers for an online retailer.</strong>
</p>

<p align="center">
  <a href="https://proactive-customer-retention.vercel.app/" target="_blank"><strong>View Live Demo</strong></a> •
  <a href="#-problem-statement">Problem Statement</a> •
  <a href="#-our-solution">Our Solution</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-running-this-project">Running Locally</a>
</p>

---

### Problem Statement

In the competitive world of e-commerce, acquiring new customers is far more expensive than retaining existing ones. Many online retailers struggle with a common challenge: **they don't know which of their customers are about to leave.** This leads to:
- **Wasted Marketing Spend:** Generic marketing campaigns are sent to everyone, failing to target the customers who actually need a nudge.
- **Lost Revenue:** Valuable customers silently churn without any intervention.
- **Lack of Insight:** The business has no clear understanding of its different customer types or their specific needs.

### Our Solution: How This Project Helps Retailers

This project provides a direct solution by turning raw sales data into an actionable business strategy. Instead of guessing, a retailer can use this analysis to:

1.  **Identify High-Value Customers:** Instantly see who their "Champion" customers are, allowing them to focus retention efforts where they will have the biggest impact.
2.  **Prevent Churn Proactively:** The predictive model flags "At-Risk" customers *before* they leave, giving the retailer a critical window to launch targeted win-back campaigns.
3.  **Personalize Marketing:** By understanding each customer segment, marketing can be tailored. Newcomers get a welcome offer, Potential Loyalists get nurtured, and Champions get rewarded. This increases engagement and conversion rates.
4.  **Make Data-Driven Decisions:** The interactive dashboard empowers the business owner to explore their own data, understand trends, and make informed decisions without needing a data scientist on hand.

---

### Our Process: From Raw Data to Actionable Insights

Our workflow was structured to ensure a robust and meaningful outcome.

<p align="center">
  <code>Data Cleaning</code> ➔ <code>RFM Analysis</code> ➔ <code>K-Means Clustering</code> ➔ <code>Churn Modeling</code> ➔ <code>Interactive Dashboard</code>
</p>

1.  **Data Cleaning & Preparation**: The initial dataset was noisy. We handled missing values, removed return transactions, and structured the data for analysis.
2.  **RFM Feature Engineering**: We created a customer "DNA" using RFM scores:
    - **R (Recency)**: How recent was their last purchase?
    - **F (Frequency)**: How often do they buy?
    - **M (Monetary)**: How much do they spend?
3.  **Unsupervised Clustering**: Using K-Means, we let the data speak for itself, revealing 4 distinct customer personas.
4.  **Predictive Modeling**: We trained a Random Forest model to predict which customers were likely to churn, allowing the business to intervene preemptively.

---

### Customer Personas Uncovered

Our analysis identified four key customer segments, each with its own unique characteristics and required strategy.

| Persona                 | Key Characteristics                                    | Recommended Action                                                              |
| :---------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------- |
|  **Champions** | Your most valuable and loyal customers. They buy often and spend the most. | **Reward them.** Offer exclusive access, loyalty points, and personalized engagement. |
|  **Potential Loyalists**| Consistent customers who show potential to become Champions. | **Nurture them.** Use targeted marketing and cross-selling to increase their frequency and spend. |
|  **Newcomers** | First-time or very recent buyers. The crucial first impression phase. | **Onboard them.** Provide a great initial experience and incentives for a second purchase. |
|  **At-Risk** | Customers who haven't purchased in a long time. High risk of leaving. | **Re-engage them.** Launch targeted "we miss you" campaigns with compelling offers to win them back. |

---

### ⚙️ Tech Stack

This project was built using a combination of data science and web development tools.

-   **Backend & Analysis**: `Python`, `Pandas`, `NumPy`, `Scikit-learn`
-   **Data Visualization**: `Matplotlib`, `Seaborn`
-   **Frontend Dashboard**: `HTML5`, `Tailwind CSS`, `JavaScript`
-   **Deployment**: `Vercel`

---

###  Running This Project

Want to explore the project on your own machine? Follow these steps.

#### 1. Clone the Repository
```sh
git clone https://github.com/OmkarY6978/customer-dashboard.git
cd customer-dashboard
```

#### 2. Install Dependencies
```sh
pip install pandas numpy scikit-learn matplotlib seaborn jupyterlab openpyxl
```

#### 3. Run the Analysis & Prepare Data
1.  Download the dataset from [Kaggle](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci) and place `online_retail_II.csv` or `.xls` in the project folder.
2.  Run the Jupyter Notebook to generate the `customer_action_plan.csv`.
3.  Run the conversion script to create the dashboard's data source:
    ```sh
    python convert_to_json.py
    ```

#### 4. View the Dashboard
Simply open the `index.html` file in your browser to see the final result.

---

<p align="center">
  <em>This project was created as a demonstration of a full-stack data science workflow, from data analysis to a user-facing product.</em>

</p>
