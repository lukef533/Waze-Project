# Waze User Churn Prediction

A machine learning project that predicts user churn for Waze using Python, data analysis, and regression modeling. This analysis provides actionable insights to support user retention strategies and improve overall user satisfaction.

## 📋 Project Overview

This project leverages exploratory data analysis, hypothesis testing, and binomial logistic regression to build a predictive model for identifying users at risk of churning. The analysis examines user activity patterns, validates behavioral assumptions, and engineers features that capture user engagement levels.

Developed to demonstrate proficiency in data science workflows, statistical analysis, and building production-ready machine learning solutions.

## Methodology

### Exploratory Data Analysis (EDA)
- Comprehensive assessment of data quality, including missing values, outliers, and duplicates
- Data visualization to identify key trends and distributions
- Focus on activity days and driving days as primary indicators of churn correlation
- Outlier imputation at the 95th percentile for enhanced model stability

### Hypothesis Testing
- Investigation of relationships between user behaviors and churn rates
- Discovery that "professional drivers" (users with higher driving frequency) exhibit lower churn rates
- Evidence-based validation of behavioral assumptions to inform feature engineering

### Feature Engineering
- Creation of derived features: `km_per_driving_day` and `professional_driver`
- Transformation of categorical variables (device type) into binary features
- Strategic feature selection to maximize predictive power and differentiate high-engagement users

### Regression Modeling
- **Model**: Binomial logistic regression
- **Approach**: Stratified sampling to address class imbalance
- **Evaluation Metrics**: Accuracy, precision, recall
- **Focus**: Recall prioritized to identify potential churn cases effectively

## Key Findings

- **User activity days** emerge as a significant negative predictor of churn—higher activity correlates with higher retention
- **Professional driver status** is a valuable feature contributing meaningfully to predictive power
- The model achieves reasonable accuracy with opportunities for refinement to improve recall
- Current model performance suggests effectiveness for some use cases, with room for optimization in capturing at-risk users

## Results

The developed model provides a foundation for identifying users at risk of churning, enabling Waze to implement targeted retention strategies. While the model demonstrates utility, its limited recall indicates potential for further enhancement.

## Future Improvements

- Additional feature engineering and evaluation of alternative machine learning algorithms
- Implementation of feature scaling techniques for improved model stability
- Integration of detailed user interaction data (geographic locations, feature engagement patterns)
- Hyperparameter tuning and cross-validation strategies
- Testing ensemble methods for enhanced predictive performance

## Repository Contents

- **Executive Summaries**: Distilled insights and recommendations for non-technical stakeholders
- **Analysis Notebooks**: Complete code for EDA, hypothesis testing, and modeling
- **Data Visualizations**: Key charts and graphs supporting analysis findings

## Tech Stack

- **Python**: Primary language for analysis and modeling
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn

## 🛠️ Technical Skills Demonstrated

**Data Analysis & Exploration**
- Exploratory Data Analysis (EDA) with comprehensive data quality assessment
- Statistical analysis of distributions, correlations, and outliers
- Data cleaning, imputation, and handling of imbalanced datasets

**Statistical Methods**
- Hypothesis testing to validate behavioral assumptions
- Correlation analysis to identify relationships between variables and outcomes
- Binomial logistic regression for binary classification

**Feature Engineering & Preprocessing**
- Creation of derived features from raw data (km_per_driving_day, professional_driver)
- Categorical variable encoding and transformation
- Outlier detection and imputation at percentile thresholds
- Stratified sampling for class imbalance management

**Machine Learning & Modeling**
- Binomial logistic regression model development and training
- Model evaluation using accuracy, precision, and recall metrics
- Hyperparameter tuning and model performance optimization
- Classification threshold analysis for business applications

**Data Visualization & Communication**
- Creation of meaningful visualizations to identify patterns and trends
- Executive summary generation for non-technical stakeholders
- Clear documentation of methodology and findings

## 🌍 Real-World Application & Business Impact

**Problem Statement**
User churn represents a significant challenge for ride-sharing and navigation apps like Waze. Understanding which users are at risk of leaving the platform enables targeted retention efforts and improved resource allocation.

**Business Value**
- **Proactive Retention**: Identify at-risk users before they churn, enabling targeted interventions such as personalized notifications, feature education, or incentive programs
- **Resource Optimization**: Focus retention efforts on high-value users (professional drivers with regular usage patterns) to maximize ROI
- **Feature Development**: Insights into user behavior patterns inform product development decisions and feature prioritization
- **Customer Lifetime Value**: Reducing churn directly improves customer lifetime value and user acquisition payback periods

**Implementation Scenarios**
- **Real-time Scoring**: Deploy the model to score active users and trigger retention campaigns for those identified as high-risk
- **Cohort Analysis**: Segment users based on churn risk for targeted engagement strategies
- **A/B Testing**: Use model insights to inform and measure effectiveness of retention initiatives
- **Predictive Analytics**: Integrate predictions into broader analytics pipelines for comprehensive business intelligence

## Conclusion

This project demonstrates the application of regression analysis to real-world data challenges, providing Waze with both technical insights and strategic recommendations for effective user retention. It reinforces the value of data-driven decision-making and supports efforts to maintain an engaged and satisfied user base.

The work showcases proficiency in building end-to-end machine learning solutions—from exploratory analysis through production-ready predictions—with clear communication of both technical rigor and business value.
