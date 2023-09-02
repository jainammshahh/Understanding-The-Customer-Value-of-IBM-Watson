# Abstract

<p align="left"> 
<a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue" alt="python" width="120" height="30"/> </a>
<a href="https://scikit-learn.org/stable/" target="_blank" rel="noreferrer"> <img src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn" width="120" height="30"/> </a>
<a href="https://scipy.org/" target="_blank" rel="noreferrer"> <img src="https://img.shields.io/badge/SciPy-654FF0?style=for-the-badge&logo=SciPy&logoColor=white" alt="scipy" width="120" height="30"/> </a>
</p>

Understanding customer behavior and predicting customer lifetime value is crucial for businesses seeking to improve customer retention and profitability. The IBM Customer Value dataset provides a comprehensive set of customer attributes that allow us to gain insights into customer demographics and interactions. This report/paper explores the prediction of customer lifetime value (CLV) using the IBM Customer Value dataset for Watson Analytics. The dataset provides relevant customer information, demographics, and buying behavior, allowing us to develop targeted customer retention programs through predictive analytics. The primary goal is to analyze customer data and understand how to retain the most profitable customers and increase their response, retention, and growth. In this study, we perform exploratory data analysis (EDA) on the dataset and consider the suitability of Principal Component Analysis (PCA) for dimensionality reduction. Efficient PCA results were obtained which were then  utilized to build models using  various predictive modeling techniques, including Generalized Linear Models (GLM), K-Means clustering, Elastic Net Regression (Lasso and Ridge), and tree-based methods such as Decision Trees, Random Forest, and Boosted Trees.

# Data Cleaning:

-   Checked for null values in the dataset and found none.
-   Examined both categorical and numeric variables for any unusual observations.
-   Plotted numeric variables to understand their distributions.
-   Dropped the "customer" column as it contained unique customer identifiers.
-   Applied label encoding to convert categorical variables into numeric values.
-   Removed outliers from the data.

# Exploratory Data Analysis (EDA): 
## A. Data Overview

-   Analyzed both categorical and numerical variables.
-   Calculated correlations between numeric variables and the target variable (Customer Lifetime Value).
-   Used barplots and boxplots to visualize relationships between categorical variables and the target.
-   Identified important variables for further analysis.

## B. Feature Selection

-   Utilized Lasso and Ridge regression tests to select important features.
-   Implemented wrapper methods like Forward and Backward selection.
-   Explored feature selection techniques due to challenges with high dimensionality.

# Principal Component Analysis (PCA):

-   Explored PCA to reduce noise, improve visualization, and perform feature engineering.
-   Experimented with different libraries and component selection to find optimal results.

# Model Analysis:

-   Tested various models including Lasso regression, Ridge regression, Generalized Linear Model (GLM), Decision Tree, Random Forest, and Gradient Boosted Trees.
-   Split the data into training and testing sets (80% and 20% respectively) for model evaluation.
-   Log normalization was applied to most models except GLM.

# Interpretation of Results:

-   Analyzed RMSE values (Root Mean Squared Error) to evaluate model performance.
-   Identified the best-performing models based on both training and testing RMSE values.
-   Considered the impact of EDA on model performance, noting that models with EDA sometimes had higher RMSE values.

# Insights:

-   Decision Tree (DT) consistently performed the best among the models, with the lowest RMSE values.
-   Random Forest (RT) and Boosted Tree (BT) showed reasonable performance.
-   GLM performed less accurately than Decision Tree.
-   EDA had a potential impact on model performance, with models with EDA sometimes having higher RMSE values.
-   Proper data cleaning, feature engineering, and model selection are crucial for accurate predictions of customer lifetime value.

The key takeaway is that the Decision Tree model proved to be the most suitable for predicting Customer Lifetime Value in the IBM Watson Marketing Customer Value dataset, while also highlighting the importance of proper data preprocessing and model selection.
