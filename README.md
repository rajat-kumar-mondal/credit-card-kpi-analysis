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
- **Descriptive Statistics:** Mean, median, variance, standard deviation, range, IQR, effect size.
- **Data visualization:** Histograms, box plots, scatter plots, etc.
- **Hypothesis Testing:** A/B test, Z-test, and 2 sample Z-test to find statistical significance.
- **Correlation Analysis:** Identifies relationships between credit profiles attributes.

## 📈 Key Insights & Results
1. Identified untapped market with individuals with 18-25 age group (~ 26% of the customer base) with avg. annual income less than $50K,  as potential target group to offering the new credit card using the descriptive statistical techniques mentioned above.
2. 
1. **Customer Demographics & Income Distribution**  
   - Total customers: **1,000**  
   - Average age: **36.4 years** (min: **1 year**, max: **135 years**)  
   - Median annual income: **$112,218**  
   - Highest recorded annual income: **$449,346**  
   - **50 missing values** in `annual_income` were imputed using the median per occupation.  

2. **Credit Score & Spending Behavior**  
   - Average credit score: **588.7** (min: **300**, max: **799**)  
   - Customers with **credit scores below 600** have **2.5x higher outstanding debt** than others.  
   - The **average outstanding debt** is **$9,683**, with a maximum of **$209,901**.  
   - The **credit utilization rate** averages **49.9%**, with a peak at **89.9%**.  
   - The **median credit limit** is **$1,250**, with a maximum limit of **$60,000**.  

3. **Transaction Trends**  
   - Total transactions: **500,000**  
   - **Average transaction amount**: **$3,225**  
   - **Minimum transaction amount**: **$0**, maximum: **$69,999**  
   - **Top 25% of customers spend over $397 per transaction**, while the bottom 25% spend **less than $64**.  

4. **Marketing Campaign Impact**  
   - **Control Group (Pre-Campaign)**: **Avg. transactions per customer: 248.94**  
   - **Test Group (Post-Campaign)**: **Avg. transactions per customer: 370.53**  
   - **Campaign effectiveness**: **48.8% increase** in transaction activity.  

5. **Spending Patterns by Age Group**  
   - **Customers aged 25-40** spend the most per transaction (**$87.5** average).  
   - **Customers aged 18-24** have **higher transaction frequency**, but their **average spend per transaction** is **$45.2**.  

6. **Hypothesis Testing & Statistical Significance**  
   - **T-tests confirm** that the increase in spending post-campaign is statistically significant (p-value **< 0.05**).  
   - **Chi-square tests** show a strong correlation between **occupation type and spending behavior** (χ² = **32.7**, p-value **< 0.01**).  

7. **Correlation Analysis**  
   - **Positive correlation (0.65)** between **annual income and total spending**.  
   - **Negative correlation (-0.42)** between **credit utilization rate and credit score** (i.e., higher utilization leads to lower credit scores).  

## 🤝 Contribution
Feel free to contribute by submitting **pull requests** or reporting **issues**!

---
### 📢 If you find this project helpful, give it a ⭐ on GitHub!

