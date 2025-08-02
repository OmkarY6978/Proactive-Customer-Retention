# Customer Retention & Churn Analysis Dashboard

<p align="center">
  <strong>A data-driven approach to understanding and retaining valuable customers for an online retailer.</strong>
</p>

<p align="center">
  <a href="https://proactive-customer-retention.vercel.app/" target="_blank"><strong>View Live Demo</strong></a> •
  <a href="#-the-challenge">The Challenge</a> •
  <a href="#-our-approach">Our Approach</a> •
  <a href="#-tech-stack">Tech Stack</a> •
  <a href="#-running-this-project">Running Locally</a>
</p>

<p align="center">
  <a href="https://proactive-customer-retention.vercel.app/" target="_blank">
    <img src="https://i.imgur.com/g9vD2mJ.png" alt="Dashboard Screenshot" width="85%">
  </a>
  <br>
  <em>An interactive dashboard built to turn complex data into actionable insights.</em>
</p>

---

### 🤔 The Challenge: Why Do Customers Leave?

For any online retailer, acquiring new customers is expensive. The real challenge lies in **customer retention**. This project tackles a critical business question: Can we identify customers who are about to leave *before* they do? Relying on guesswork leads to wasted marketing budgets and lost revenue. We need a way to pinpoint at-risk customers and understand our most loyal ones to act effectively.

### ✨ Our Approach: A Proactive Strategy

This project moves beyond simple sales reporting to build a proactive retention engine. By analyzing over a year of transactional data, we developed a system that:

1.  **Segments customers** into meaningful groups based on their purchasing behavior.
2.  **Predicts churn risk** using a machine learning model.
3.  **Provides clear, actionable recommendations** through an interactive dashboard designed for business decision-makers.

---

### 🗺️ Our Process: From Raw Data to Actionable Insights

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

### 👥 Customer Personas Uncovered

Our analysis identified four key customer segments, each with its own unique characteristics and required strategy.

| Persona                 | Key Characteristics                                    | Recommended Action                                                              |
| :---------------------- | :----------------------------------------------------- | :-------------------------------------------------------------------------------- |
| 🏆 **Champions** | Your most valuable and loyal customers. They buy often and spend the most. | **Reward them.** Offer exclusive access, loyalty points, and personalized engagement. |
| ⭐ **Potential Loyalists**| Consistent customers who show potential to become Champions. | **Nurture them.** Use targeted marketing and cross-selling to increase their frequency and spend. |
| 🌱 **Newcomers** | First-time or very recent buyers. The crucial first impression phase. | **Onboard them.** Provide a great initial experience and incentives for a second purchase. |
| ⚠️ **At-Risk** | Customers who haven't purchased in a long time. High risk of leaving. | **Re-engage them.** Launch targeted "we miss you" campaigns with compelling offers to win them back. |

---

### ⚙️ Tech Stack

This project was built using a combination of data science and web development tools.

-   **Backend & Analysis**: `Python`, `Pandas`, `NumPy`, `Scikit-learn`
-   **Data Visualization**: `Matplotlib`, `Seaborn`
-   **Frontend Dashboard**: `HTML5`, `Tailwind CSS`, `JavaScript`
-   **Deployment**: `Vercel`

---

### 🚀 Running This Project

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