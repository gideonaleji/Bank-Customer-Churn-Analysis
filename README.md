# 🏦 Bank Customer Churn Prediction Analysis


<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-learn" />
  <img src="https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge&logo=xgboost&logoColor=white" alt="XGBoost" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI" />
  <img src="https://img.shields.io/badge/Logistic%20Regression-007ACC?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyBmaWxsPSJ3aGl0ZSIgaGVpZ2h0PSIyMCIgd2lkdGg9IjIwIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciLz4=" alt="Logistic Regression" />
  <img src="https://img.shields.io/badge/Decision%20Tree-228B22?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyBmaWxsPSJ3aGl0ZSIgaGVpZ2h0PSIyMCIgd2lkdGg9IjIwIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciLz4=" alt="Decision Tree" />
</div>



## 📋 Table of Contents

- [🧠 Project Overview](#-project-overview)
- [🔍 Key Findings](#-key-findings)
- [📊 Dataset Description](#-dataset-description)
- [⚙️ Technologies & Tools](#️-technologies--tools)
- [📈 Model Performance](#-model-performance)
- [🔬 Feature Analysis](#-feature-analysis)
- [💡 Business Insights](#-business-insights)
- [📌 Recommendations](#-recommendations)
- [⚠️ Data Limitations & Future Data Enhancements](#️-data-limitations--future-data-enhancements)
- [🖼 Dashboard](#-dashboard)
- [🎯 Impact Assessment](#-impact-assessment)
- [👤 Author](#-author)
- [📄 License](#-license)


## 🧠 Project Overview

The aim of this project is to predict customer churn in a banking institution using machine learning algorithms. The goal is to develop a predictive model that can identify which customers are at high risk of leaving the bank based on the demographic, financial, and behavioural data provided. By understanding the key drivers behind customer attrition, the bank can develop proactice strategies to retain valuable clients and reduce churn rates. 

Customer churn is a significant threat to financial institutions, not only in lost revenue but also in increased costs associated with acquiring new customers. This analysis seeks to address the problem by accurately identifying churn-prone customers, understanding the underlying causes of churn, and offering actionable recommendations to prevent it.


## 🔍 Key Findings

The results of the analysis revealed a high churn rate of 54.4%, indicating that more than half of the bank's customers are leaving. This is a major red flag and suggests urgent intervention is needed from the bank leadership. A detailed demographic and behavioural analysis showed that male customers are 60% more likely to churn than females, and customers without credit cards also demonstrated a much higher tendency to leave.

Geographic data revealed that France experiences the highest churn rates among all regions analyzed, suggesting that regional service delivery might be affecting customer satisfaction. Moreover, tenure and engagement metrics such as activity level and the number of products held by a customer significantly influenced their likelihood to churn.


![Screenshot 2025-07-09 171723](https://github.com/user-attachments/assets/2f3032fa-7c9c-4018-bf3f-afc39a56cbed)



![Screenshot 2025-07-09 171619](https://github.com/user-attachments/assets/5c5ddc68-6107-4a1c-a492-76db2c1bc44c)



## 📊 Dataset Description

The dataset consists of 500 customer records with 13 features capturing demographic, financial, and behavioural characteristics. The target variable is binary (0 for retained, 1 for churned). Data quality was generally good, with three missing salary values addressed using median imputation and one invalid balance entry corrected during preprocessing.

The feature categories include:

- Demographic: Age, Gender, Geography
- Financial: Credit Score, Balance, Estimated Salary
- Behavioural: Tenure, Number of Products, Credit Card Ownership, Active Membership


## ⚙️ Technologies & Tools

The analysis was performed using Python. Core libraries included:

- *Pandas and Numpy* for data manipulation
- *Scikit-learn, XGBoost, and other models* for machine learning
- *Matplotlib and Seaborn* for visualizations
- *Jupyter Notebook* for interactive development
- *PowerBI* for dashboarding

The models tested included Logistic Regression, Decision Tree, Random Forest, K-Nearest Neighbors, XGBoost, and Support Vector Machine (SVM).


## 📈 Model Performance

Among all the models tested, *Logistic Regression* achieved the highest performance with an accuracy of 53%, precision of 0.55, recall of 0.58, and F1-score of 0.57. It also offered the best trade-off between interpretability and performance, making it ideal for business stakeholders.

Other models such as K-Nearest Neighbours and Decision Trees performed moderately well while XGBoost and SVM did not perform as expected, likely due to the relatively small dataset and the imbalance between churn and non-churn classes.

THe models were evaluated on various metrics, and performance was visualized to compare strengths and weaknesses. Feature selection and engineering attempts did not significantly improve results, hightlighting the limitations of the dataset.


## 🔬 Feature Analysis

The analysis of feature importance (especially from tree-based models) revealed that the following variables played the most significant roles in predicting churn:

1. Balance
2. Estimated Salary
3. Credit Score
4. Age
5. Tenure

Balance, in particular, was the strongest predictor, with lower balance customers being a more likely to churn. A visualization of feature importance helped solidify these insights and guided the business recommendations provided.


![Screenshot 2025-07-09 171803](https://github.com/user-attachments/assets/dcdaaf83-b406-41ef-bf76-2f35f8d89299)


## 💡 Business Insights

Several business insights emerged from the data:

- *Credit Card ownership* strongly correlates with customer retention. Customers without credit cards are more likely to churn.
- *Inactive customers* show a much higher likelihood of leaving, suggesting that engagement plays a critical role.
- *Male customers*, as well as those in France, are disproportionately represented among those who leave.
- *Customers with fewer products and lower tenure* are also high-risk.

These insights can guide targeted marketing, operational changes, and policy adjustments.


## 📌 Recommendations

The following actions are my reommendations to reduce churn:

### Immediate Actions

- Excecutive intervention is needed to address the alarming churn rate. A task force should be formed to allocate resources and develoop emergency strategies.
- Investigate the French market and resolve operational issues that may be contributing to poor retention.
- Promote credit card ownership and product engagement through incentivized campaigns.

### Strategic Programs

- Implement customer segmentation to target high-risk groups with tailored retention strategies.
- Launch loyalty programs and offer benefits to customers based on tenure and engagement.
- Improve the customer experience across channels, particularly digital platforms and customer support services.


## ⚠️ Data Limitations & Future Data Enhancements

While the current dataset provided a useful starting point for churn analysis, it proved to be significantly limited in scope. The dataset contained only 500 customer records with 13 basic attributes, primarily covering static demographic and financial information such as age, gender, credit score, balance, and product holdings. WHile these features offer some predictive power, they are insuggicient for capturing the dynamic and behavioural patterns that typically influence customer churn.

The relatively poor performance of all machine learning models, with the best achieving only 53% accuracy, can be largely attributed to this data insufficiency. For more accurate and actionable churn prediction, future iterations of this analysis should include richer and more granular data.

### 🔄 Recommended Features for Future Data Collection

To enhance the quality of insights and improve predictive accuracy, the following types of data are recommended for future inclusions:

#### 🧾 Customer Behavior & Activity

Tracking how customers interact with the bank can reveal early signs of disengagments:

- Frequency of online banking logins
- ATM and branch visit counts
- Monthly transaction volume
- Last transaction or login date
- Number of customer service interactions or complaints

#### 💰 Product and Service Engagement

Understanding the depth of customer relationships across multiple services:

- Types of accounts held (e.g., savings, checking, fixed deposit)
- Usage of loan, mortgage, or insurance products
- Investment accounts or mutual fund subscriptions
- Recent product upgrades or closures
- Loyalty program participation and offer redemptions

#### 📉 Trend-Based Metrics

Churn is often preceded by gradual behavioural shifts. Including temporal features can be extremely valuable:

- Change in account balance over the past 3-6 months
- Trends in salary deposits
- Decline in product usage over time
- Drop in customer engagement or transaction frequency

#### 🧑‍💼 Relationship & Satisfaction Indicators

Customer sentiment and relationship health often predict future churn:

- Satisfaction survey scores
- Net Promoter Score (NPS)
- Tenure with assigned relationship manager
- History of escalated issues or unresolved complaints

#### 📈 Impact of Enhanced Data

Including these additional features will not only improve model performance but also enable more nuanced customer segmentation and targeted interventions. With richer data, machine learning models can detect complex patterns that are currenly invisible, allowing for more timely and effective churn prevention strategies.


## 🖼 Dashboard

Below is the final dashboard for the project. It was designed in PowerBI.


![Screenshot 2025-07-08 222834](https://github.com/user-attachments/assets/fae4a527-daec-4e04-8666-301db88d12d4)


## 🎯 Impact Assessment

With a current churn rate of 54.4%, any improvement will have a significant revenue impact. If the bank can reduce churn to 5-10% (the industry average), it stands to retain a substantial portion of lost revenue and increase customer lifetime value. Metrics for success include:

- Reduced churn rate
- Increased product adoption (e.g., credit card ownership)
- Improved customer engagement and satisfaction


## 👤 Author

Gideon Aleji

📧 Email: alejigideonabidemi@gmail.com
💼 LinkedIn: [(https://www.linkedin.com/in/gideon-aleji-4b7073354/)]
🐱 GitHub: [(https://github.com/gideonaleji)]


## 📄 License

This project is licensed under the MIT License.


<div align="center"> <strong>⭐ If you found this project useful, please consider starring it on GitHub! ⭐</strong> </div>



##
