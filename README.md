Automobile Pricing and Credit Card Customer Segmentation
Overview

This project encompasses two distinct data analysis tasks:

    Automobile Pricing: A linear regression analysis to predict the resale price of Toyota Corolla vehicles based on their features.
    Credit Card Customer Segmentation: A clustering analysis to segment bank customers based on their creditworthiness, providing actionable insights for targeted marketing of a new low-interest personal loan.

The project applies advanced data cleaning, statistical modeling, and clustering techniques to derive insights from the provided datasets.
Objectives
Automobile Pricing

    Identify the key factors influencing the resale price of Toyota Corolla cars.
    Evaluate the statistical significance of vehicle features like age, mileage, manufacturing year, and fuel type.
    Interpret the regression model to provide actionable insights for car dealerships.

Credit Card Customer Segmentation

    Segment customers based on their creditworthiness using clustering techniques.
    Determine the most creditworthy cluster for targeted marketing of a new financial product.
    Evaluate the effectiveness of the clustering model using mathematical metrics and business context.

Datasets
Automobile Pricing

    ToyotaCorolla.xlsx: Contains 1,436 rows and multiple columns with data on used Toyota Corolla cars.
        Variables:
            Vehicle_Age: Age of the car (in years).
            KM: Mileage (in kilometers).
            Mfg_Year: Manufacturing year.
            Price: Resale price of the car.
            Fuel_Type: Type of fuel used (e.g., Petrol, Diesel, CNG).

Credit Card Customer Segmentation

    CC GENERAL.csv: Contains customer transaction data for credit card accounts.
        Variables include:
            BALANCE: Outstanding balance.
            PURCHASES: Total purchases made.
            CREDIT_LIMIT: Credit limit assigned to the customer.
            MINIMUM_PAYMENTS: Minimum payments made by the customer.

Methodology
Automobile Pricing

    Data Cleaning:
        Selected relevant variables (Price, Vehicle_Age, KM, Mfg_Year, Fuel_Type).
        Converted Fuel_Type to dummy variables for regression.
        Checked and imputed missing values (if any).

    Linear Regression:
        Conducted regression analysis to predict Price.
        Evaluated model performance using adjusted R-squared.
        Identified statistically significant predictors using p-values.

    Interpretation:
        Assessed the impact of mileage, manufacturing year, and fuel type on price.

Credit Card Customer Segmentation

    Variable Selection:
        Chose variables relevant to creditworthiness, such as BALANCE, PURCHASES, and CREDIT_LIMIT.
        Excluded highly correlated variables to improve clustering performance.

    Data Cleaning:
        Imputed missing values in CREDIT_LIMIT and MINIMUM_PAYMENTS.
        Normalized the data to ensure equal weight for all variables.

    Clustering Analysis:
        Used the elbow method to determine the optimal number of clusters (k=3).
        Performed K-means clustering to segment customers.

    Cluster Evaluation:
        Evaluated cluster performance using the Silhouette Score and business meaningfulness.
        Described customer types within each cluster and identified the most creditworthy segment.

Results
Automobile Pricing

    Adjusted R-squared: 0.808, indicating that the model explains 80.8% of the variance in resale prices.
    Significant Variables:
        KM (Mileage): Higher mileage decreases price.
        Mfg_Year (Manufacturing Year): Newer cars have higher prices.
        Fuel_Type (Diesel): Diesel cars have higher resale prices than CNG.
    Insights provided actionable recommendations for pricing strategies.

Credit Card Customer Segmentation

    Optimal Clusters: 3
        Cluster 0: High-balance customers with frequent cash advances.
        Cluster 1: Low-balance, low-activity customers.
        Cluster 2: Moderate-balance, high-activity customers (most creditworthy).
    Silhouette Score: 0.29, indicating moderate cluster separation.
    Recommendations enabled targeted marketing of the new loan product.

Tools and Technologies

    Python: For data cleaning, regression analysis, and clustering.
        Libraries: pandas, numpy, sklearn, matplotlib, seaborn.
    Jupyter Notebook: For interactive coding and analysis.
    Microsoft Excel: For dataset review and manual adjustments.

Instructions for Use

    1. Clone the repository:git clone https://github.com/YourUsername/AutoPrice-CreditSegmentation.git
    2. Open the Jupyter Notebooks:
        Assignment 3 A.ipynb: For Automobile Pricing analysis.
        Assignment 3 B.ipynb: For Credit Card Customer Segmentation.
    3. Follow the provided code and documentation to replicate the analyses.

Acknowledgments
This project was completed as part of the MKT 568 coursework at WPI Business School. Special thanks to the course instructor for her guidance and support.


