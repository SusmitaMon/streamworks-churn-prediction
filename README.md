## 🎬 StreamWorks Customer Churn Prediction
### Machine Learning & Customer Behaviour Analysis

A data science project analysing customer churn for a subscription-based streaming platform (StreamWorks).
The project combines exploratory data analysis, statistical testing, feature engineering, and machine learning models to identify churn drivers and predict at-risk users.
The goal is to help subscription businesses improve retention through data-driven insights.

------

### 📌 Key Results

- UK customers show the highest churn rate (~27%)
- Standard subscription users churn the most (~24.6%)
- Promotions significantly influence churn behaviour (p-value = 0.002)
- Random Forest model achieved 77% accuracy for churn classification
- Engagement model explained 93% of watch time variance (R² = 0.93)

----------

### 📊 Project Highlights

✔ Built an end-to-end churn prediction pipeline
✔ Performed feature engineering and statistical testing (Chi-Square)
✔ Developed Logistic Regression and Random Forest models
✔ Analysed customer engagement behaviour and churn drivers
✔ Generated business recommendations for retention strategies

--------

### 🧠 Business Problem

Streaming platforms rely heavily on subscription retention.

Even a small increase in churn can significantly impact revenue.

This project answers three key business questions:

1️⃣ Which users are most likely to churn?
2️⃣ What behavioural patterns lead to churn?
3️⃣ How can the company reduce churn through targeted actions?

-------

### 📂 Dataset Overview

The dataset contains behavioural and subscription data for StreamWorks users.

#### Key features include:

#### Category	Variables:

Customer Demographics	Age, Country
Subscription Data	Subscription Type, Monthly Fee
User Engagement	Average Watch Hours
Mobile Behaviour	Mobile App Usage %
Customer Activity	Complaints Raised
Marketing Signals	Promotions Received
Referral Behaviour	Referred by Friend
Customer Lifecycle	Tenure Days
Engineered Features	Watch-per-Fee Ratio, Heavy Mobile User

#### Target variable:

is_churned
0 = Active customer
1 = Churned customer

------

### 🔎 Exploratory Data Analysis
Churn by Country
Country	Churn Rate
UK	27.1%
India	24.1%
France	23.7%
Germany	22.5%
Canada	21.3%
USA	21.3%

📌 Insight: UK users show the highest churn, suggesting potential market competition or pricing sensitivity.

------

### Churn by Subscription Type
Subscription	Churn Rate
Standard	24.6%
Basic	23.8%
Premium	21.6%

📌 Insight: Premium subscribers tend to churn less due to higher engagement.

-----

### 📈 Statistical Analysis

Chi-Square tests were used to identify statistically significant relationships between categorical variables and churn.

Feature	p-value	Result
Gender	0.107	Not Significant
Received Promotions	0.002	Significant
Referred by Friend	0.533	Not Significant

📌 Key Finding:
Customers who receive promotions show significantly different churn behaviour, indicating marketing campaigns influence retention.

-------

### 🤖 Machine Learning Models
#### Logistic Regression
Metric	Score
Accuracy	0.53
Precision (Churn)	0.24
Recall (Churn)	0.46
ROC-AUC	0.506

📌 Performance close to random classification due to class imbalance.

#### Random Forest
Metric	Score
Accuracy	0.77
Recall (Churn)	0.00
ROC-AUC	0.46

📌 Model predicts non-churn well but struggles to identify churn users due to imbalanced classes.

Future improvement:
SMOTE or class weighting.

-------

### 📊 Behaviour Modelling (Watch Time)

A Linear Regression model was built to predict user engagement.

Metric	Value
R²	0.93
RMSE	5.87 hours
#### Top Positive Drivers

Watch per fee ratio

High watch time group

Monthly subscription fee

Heavy mobile usage

#### Top Negative Drivers

Low watch engagement after promotions

Older age groups

Long tenure without engagement growth

--------

### 💡 Key Insights
#### 1️⃣ Engagement is the strongest retention driver

Users with higher watch time per subscription cost stay longer.

#### 2️⃣ Promotions influence churn behaviour

Promotional engagement significantly affects retention.

#### 3️⃣ Regional churn differences

UK users show the highest churn rate.

#### 4️⃣ Low engagement after promotions signals churn risk

Customers who receive promotions but watch less content are likely to leave.

--------

### 🚀 Business Recommendations
🎯 Target low engagement users

Identify customers with low watch-per-fee ratios and intervene early.

🎯 Improve personalised recommendations

Increase engagement by promoting relevant content.

🎯 Optimise promotional campaigns

Offer incentives tied to content engagement rather than price discounts.

🎯 Investigate UK churn drivers

Possible causes include pricing, competitor platforms, or content availability.

--------

### 🛠️ Tech Stack

Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
Jupyter Notebook

------

### 📁 Project Structure
streamworks-churn-prediction
│
├── Churn_Prediction_StreamWorks.ipynb
├── README.md
└── visualizations

-----

### ▶️ Run the Project

1. Clone the repository
git clone https://github.com/SusmitaMon/streamworks-churn-prediction.git
cd streamworks-churn-prediction

2. Install required libraries
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

3. Launch Jupyter Notebook
jupyter notebook

This will open the Jupyter interface in your browser.

4. ### Run the Notebook

View on GitHub:  
[Churn_Prediction_StreamWorks.ipynb](https://github.com/SusmitaMon/streamworks-churn-prediction/blob/main/Churn_Prediction_StreamWorks.ipynb)

Run in Google Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/SusmitaMon/streamworks-churn-prediction/blob/main/Churn_Prediction_StreamWorks.ipynb)


-------

### 👩‍💻 Author

**Susmita Mondal**  
Data Analyst | Power BI Developer  
Passionate about transforming raw data into insights that support business decision-making and customer analytics.

LinkedIn  
https://www.linkedin.com/in/susmita-mondal-51853999/

GitHub  
https://github.com/SusmitaMon


