Telco Customer Analysis Project

This project explores the Telco Customer Churn dataset to understand customer behavior and predict churn. We go through a complete data science workflow, including data exploration, cleaning, preparing data for modeling, building different types of models (regression, classification, and clustering), and finally, interpreting the results to offer practical recommendations for the business.

The dataset comes from Kaggle: [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data).

 Project Steps:

1.  Data Loading: We start by loading the dataset and getting a feel for its structure and contents.

2.  Data Cleaning & Preparation: This involves handling missing values, making sure data types are correct, encoding categories, and scaling numerical data so our models can understand it better.

3.  Exploring the Data (EDA): We dive into the data to find patterns. This includes:
    *   Looking at key statistics.
    *   Visualizing how many customers have churned.
    *   Seeing how different features relate to each other using a heatmap.
    *   Checking the distributions of numerical features with plots.

4.  Predicting Monthly Charges (Regression): We build models to predict how much a customer's monthly bill will be. We use Linear Regression and Random Forest Regression and check how well they perform using metrics like MAE, RMSE, and R².

5.  Predicting Churn (Classification): Here, the goal is to predict whether a customer is likely to leave. We use Logistic Regression, Random Forest, Decision Tree, and LightGBM models. We evaluate them using metrics like the confusion matrix, F1 score, and ROC-AUC score to see which one is best at identifying customers who might churn. We also address class imbalance to make sure our model isn't biased.

6.  Customer Segmentation (Clustering): We group customers based on their behavior using K-Means clustering. We use PCA to help visualize these groups and evaluate the quality of our clusters using the Silhouette Score.

7.  Business Insights and Recommendations: Based on everything we've learned from the analysis and the models, we provide insights into customer behavior and suggest actions the telecom company can take to improve customer retention and business strategy.

 Insights:

*   A complete analysis covering:
    *   Detailed data exploration.
    *   Models for regression (predicting monthly charges), classification (predicting churn), and unsupervised learning (segmenting customers).
    *   A section with clear business insights and recommendations.

  Analysis Highlights:

*   EDA Insights: Identified specific services (like fiber optic and month-to-month contracts) and payment methods (electronic check) associated with higher churn risk. Also saw that higher monthly charges seem linked to churn, while customers who stay tend to have higher total charges due to longer tenure.

*   Regression Model: The Random Forest Regressor did a good job predicting monthly charges. This can help the business understand what influences charges and forecast revenue.

*   Classification Model: The Random Forest Classifier (after tuning) performed well in predicting churn, providing a way to identify at-risk customers.

*   Clustering Insights: Grouped customers into distinct segments based on tenure, monthly charges, and total charges, revealing groups of loyal high-value customers, new customers, and potentially at-risk high-spending new customers.

   Recommendations:

*   Focus on Loyalty: Implement programs to keep high-value, long-term customers happy (Segments 0 and 2).

*   Prevent Churn: For newer customers (Segments 1 and 3), offer onboarding support and early incentives to build loyalty.

*   Address Churn Drivers: Consider promotions or alternative options for services and contract types strongly linked to churn.
*   Track Customer Journey: Monitor how customers move between segments to better understand their lifecycle and anticipate needs.

This project provides a solid foundation for the Telco company to make data-driven decisions to reduce churn and improve customer satisfaction.