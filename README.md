# Springboard-Course-Capstone-Project-1
                              Survival Analysis on Telco Customer Churn
                                      
                                      Executive Summary

Customer churn, defined as the percentage of customers that stop using a company's products or services, is one of the most import matrices for a business, as it usually costs more to acquire new customers than it does to retain existing ones.

The dataset of Telco customer churn was acquired from Kaggle competition website. The client is the management of the pertaining business. The objective of this project is to predict if customers are likely to stop doing business and when that event might happen.  With the model built and data analysis performed, the business owners will be able to segment the customers based on the likelihood to churn and take appropriate actions to prevent that happening, such us launching customer retention program. 

To perform survival analysis on such a time-event problem, we will treat the features of “tenure” and “churn” as target variable. During the process of data wrangling, we explored how each variable is distributed individually and how they are correlated with each other. Since the most of variables are of categorical type, we used Cramer'V to explore correlation for categorical variables, whereas Pearson correlation for numerical ones. 

There are multiple algorithms built in Scikit-survival to perform survival analysis. First of all, we used the non-parametric method Kaplan–Meier estimator to find out how “tenure” affects the likelihood of customer churn by plotting survival function curve.  However, semi-parametric method Cox Proportional Hazard is more powerful to predict whether a customer churn based on not only time factor but also other attributes. In order to achieve better performance, we applied feature selection techniques to figure out the importance of each variables in building the predictive model.  L1-based feature selection CoxnetSurvivalAnalysis and univariate feature selection using SelectKBest were used in this project. 

Furthermore, some other advanced algorithms such as survival tree, survival random forest, survival support vector machine, survival kernel support vector machine and gradient boosting survival analysis were also be explored in this project.
