# 📌 Credit Card KPI Analysis

## 📖 Overview
This project conducts a statistical analysis of key performance indicators (KPIs) in credit card usage to identify a new target group to whom we can offer the credit card, with a high likelihood that they will use it. Using real-world transaction data, customer profiles, and post-campaign insights, it aims to identify trends, spending behaviors, new target customer groups, and the impact of marketing campaigns.

## 📂 Project Structure
```
/
credit_card_KPI_analysis.ipynb           # Jupyter Notebook for full analysis

data/
│   ├── credit_profiles.csv              # Credit profile details of customers
│   ├── customers.csv                     # Customer demographics
│   ├── transactions.csv                   # Credit card transaction history
│   ├── data_after_campaign/
│       ├── avg_transactions_after_campaign.csv  # Post-campaign transaction data
```

## ⚡ Key Features
- **Exploratory Data Analysis (EDA)**: Insights into credit card spending habits.
- **Spending Pattern Analysis**: Analysis of different customer groups based on spending patterns.
- **Target Group Finding:** Finding the target group to offer the new credit card, ensuring they cannot reject it and will actively use it.
- **Campaign Impact Analysis**: Evaluates how marketing campaigns affect credit card usage through hypothesis testing.


## 🛠 Installation & Usage
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/credit-card-KPI-analysis.git
cd credit-card-kpi-analysis
```

### 2️⃣ Install Dependencies
```bash
pip install numpy pandas matplotlib seaborn statsmodels
```

### 3️⃣ Run the Jupyter Notebook
```bash
jupyter notebook credit_card_kpi_analysis.ipynb
```

## 📊 Dataset
The dataset contains transactional and demographic data, including:
- **`customers.csv`**: Customer details (1K records) such as age, occupation, and annual income.
- **`credit_profiles.csv`**: Such as credit score and risk classification (1K+ records).
- **`transactions.csv`**: Detailed transaction records (half-million).
- **`avg_transactions_after_campaign.csv`**: Insights into transactions post-marketing campaign (62 records).

## 🔬 Statistical Methods Used
- **Descriptive Statistics:** Mean, median, variance, standard deviation, range, IQR, statistical power, and effect size.
- **Data visualization:** Histograms, box plots, scatter plots, etc.
- **Hypothesis Testing:** A/B test, Z-test, and 2 sample Z-test to find statistical significance.
- **Correlation Analysis:** Identifies relationships between credit profiles attributes.

## 📈 Key Insights & Results
1. Identified an untapped market within the 18–25 age group (~26% of the customer base) with an average annual income of less than $50K (with limited credit history and low credit card usage) as a potential target group (test group) for offering the new credit card using the descriptive statistical techniques mentioned above.
2. Found that Electronics, Fashion & Apparel, and Beauty & Personal Care are the top three shopping categories for the target group using the same techniques.
3. Identified the optimal sample size that balances cost efficiency and statistical reliability for the campaign, with a statistical power of 80% and an effect size of 2.
4. Designed hypotheses (i.e., H0 and Ha) and tested them using the hypothesis testing techniques mentioned above, rejecting the null hypothesis with 95% confidence. By accepting Ha, we found that the average transaction amount for the test group is greater than that of the control group.
5. Based on the findings, we can launch the credit card exclusively in the market for the 18–25 age group.

---

