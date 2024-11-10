# Waze User Churn Prediction Project

In this project, I developed a machine learning model to predict user churn for Waze, utilizing Python for data exploration, hypothesis testing, and regression analysis. My goal was to analyze user activity data, extract meaningful insights, and create a predictive model to support Waze’s strategy for improving user retention and overall user satisfaction.
Project Overview

### 1. Exploratory Data Analysis (EDA)
The project begins with a comprehensive Exploratory Data Analysis (EDA) phase, where I delve into Waze's user data to understand its structure and identify any underlying patterns. I assessed data quality by checking for missing values, potential outliers, and duplicates, ensuring a solid foundation for my analysis. Through various data visualizations, I identified important trends and distributions, noting that activity days and driving days, in particular, show correlations with user churn. To address extreme values and enhance the model's stability, I imputed outliers at the 95th percentile for specific variables.

### 3. Hypothesis Testing
Following EDA, I conducted a hypothesis test to investigate the relationship between user behaviors and churn rates. For example, I discovered that "professional drivers"—users with a higher frequency of driving days—tend to have lower churn rates. This insight informed my feature engineering process, allowing me to tailor features to strengthen the model’s predictive power. Hypothesis testing provided an evidence-based approach to validate assumptions, adding rigor to my model development.

### 4. Feature Engineering
In the feature engineering phase, I leveraged insights from EDA and hypothesis testing to create additional variables that enhanced the predictive capabilities of the model. I introduced km_per_driving_day and professional_driver to capture unique aspects of user behavior, helping to differentiate high-engagement users. I also transformed categorical variables, such as device type, into binary features suitable for model input. This process ensured that my model captured relevant information in a format that maximized predictive power.

### 5. Regression Modeling
To predict user churn, I selected a binomial logistic regression model, which estimates the probability of churn based on multiple user attributes. The model was trained on a subset of the data, and I managed class imbalance through stratified sampling to ensure the model was well-calibrated. During evaluation, I examined key metrics like accuracy, precision, and recall, with a particular focus on recall given the importance of identifying potential churn cases. The model's accuracy provided a general measure of performance, while precision and recall highlighted its effectiveness in correctly identifying users likely to churn.

### 6. Results & Insights
From my model, I uncovered that user activity days are a significant negative predictor of churn, indicating that higher activity is associated with higher retention. "Professional_driver" status also emerged as a valuable feature, contributing positively to the model's predictive power. Although the model achieved reasonable accuracy, its limited recall highlighted opportunities for further refinement. This insight suggested that while the model is useful for some purposes, additional optimization could improve its performance, especially in capturing users on the verge of churning.

### 7. Executive Summaries
For convenience and clarity, executive summaries containing key findings, insights, and recommendations are available in this repository. These summaries distill complex model results into actionable insights, making them accessible to non-technical stakeholders and supporting data-driven decision-making at Waze.
Next Steps

Moving forward, I plan to explore several avenues for model improvement. Additional feature engineering and testing with other machine learning models could help optimize prediction accuracy. Applying feature scaling techniques may enhance model stability and predictive power. Additionally, incorporating more detailed user interaction data—such as geographic locations of drives or engagement with app features like road hazard alerts—could further increase the model's ability to predict churn accurately.
This project demonstrates the application of regression analysis to real-world data, providing Waze with both technical insights and strategic recommendations for addressing user churn effectively. This approach not only reinforces the value of data-driven decision-making but also supports Waze’s mission to retain an engaged and satisfied user base.





