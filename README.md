Customer Churn Prediction Project
Overview
The objective of this project was to predict customer churn for a subscription-based business using machine learning. By identifying high-risk customers, the business can implement targeted retention strategies to minimize churn and maximize revenue.

Steps Taken
Dataset Preparation:

A realistic dataset was generated, containing customer demographics, behavior, and subscription details.
Key features included monthly spend, tenure, recent activity, and payment methods.
Exploratory Data Analysis (EDA):

Identified patterns and trends in churn-related features:
Higher churn among customers with shorter tenure or higher monthly spend.
Lower recent activity was a strong indicator of churn risk.
Visualized distributions, correlations, and feature relationships to guide preprocessing and modeling.
Data Preprocessing:

Handled class imbalance using SMOTE (Synthetic Minority Oversampling Technique) to ensure fair representation of churners in the training data.
Encoded categorical variables and scaled numerical features for model compatibility.
Model Training:

Trained multiple machine learning models:
Logistic Regression
Random Forest
XGBoost
Evaluated model performance using metrics such as accuracy, precision, recall, and F1-score.
Feature Importance Analysis:

Analyzed the Random Forest model’s feature importance to identify the most significant predictors of churn.
Challenges and How We Tackled Them
Class Imbalance:

Problem: The dataset had far fewer churners (1) compared to non-churners (0), leading to biased predictions.
Solution: Applied SMOTE to oversample churners, improving the model’s ability to predict churn effectively.
Low Recall for Churn Prediction:

Problem: Initial models struggled to recall churners, with predictions heavily favoring non-churners.
Solution: Balancing the dataset with SMOTE significantly improved recall for churners across models.
Feature Selection:

Problem: Determining which features contributed most to churn prediction.
Solution: Used feature importance analysis from the Random Forest model to prioritize impactful variables like MonthlySpend, RecentActivityDays, and Income.
Key Insights
Top Predictors of Churn:

MonthlySpend: High monthly expenses were strongly associated with churn, highlighting the need for cost optimization strategies.
RecentActivityDays: Customers with low recent activity were at greater risk of churn, emphasizing the importance of engagement.
Income: Lower-income customers were more likely to churn, suggesting affordability concerns.
Customer Behavior and Retention:

Short-tenure customers were more likely to churn, pointing to the importance of strong onboarding experiences.
Frequent support tickets indicated unresolved issues leading to dissatisfaction.
Segment-Specific Strategies:

Tailored discounts for high-spend customers.
Re-engagement campaigns for low-activity customers.
Improved customer service for users with multiple support interactions.
Impact
Improved Churn Recall: The Random Forest model with SMOTE achieved better recall for churners, ensuring high-risk customers are effectively identified.
Actionable Insights: The feature importance analysis provided clear directions for targeted retention strategies.
Future Enhancements
Hyperparameter tuning to further optimize model performance.
Incorporating additional behavioral features, such as customer feedback or loyalty scores.
Real-time prediction and monitoring using dashboards for business decision-making.
