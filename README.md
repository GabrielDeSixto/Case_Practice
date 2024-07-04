# DMResources Limited - Personalized Micro Credits

## Overview

This project aims to analyze and predict customer churn for DMResources Limited, a Fintech company in Mexico offering personalized microcredits to small and medium businesses. The analysis and model aim to comply with Mexican regulations and reduce churn to optimize profit.

## Data Description

The data consists of three tables:
1. **Charges**: Contains information about the monthly and total charges for each customer.
2. **Other data**: Contains demographic and service-related information for each customer.
3. **Churn**: Indicates whether each customer has churned.

### Data Dictionary

- **customerID**: Customer ID
- **gender**: Gender of the customer (Male, Female)
- **SeniorCitizen**: Whether the customer is a senior citizen (1, 0)
- **Partner**: Whether the customer has a partner (Yes, No)
- **Dependents**: Whether the customer has dependents (Yes, No)
- **Tenure**: Number of months the customer has stayed with the company
- **PhoneService**: Whether the customer has phone service (Yes, No)
- **MultipleLines**: Whether the customer has multiple lines (Yes, No, No phone service)
- **InternetService**: Customer’s internet service provider (DSL, Fiber optic, No)
- **OnlineSecurity**: Whether the customer has online security (Yes, No, No internet service)
- **OnlineBackup**: Whether the customer has online backup (Yes, No, No internet service)
- **DeviceProtection**: Whether the customer has device protection (Yes, No, No internet service)
- **TechSupport**: Whether the customer has tech support (Yes, No, No internet service)
- **StreamingTV**: Whether the customer has streaming TV (Yes, No, No internet service)
- **StreamingMovies**: Whether the customer has streaming movies (Yes, No, No internet service)
- **Contract**: The contract term of the customer (Month-to-month, One year, Two year)
- **PaperlessBilling**: Whether the customer has paperless billing (Yes, No)
- **PaymentMethod**: The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- **MonthlyCharges**: The amount charged to the customer monthly
- **TotalCharges**: The total amount charged to the customer
- **Churn**: Whether the customer churned (Yes, No)

## Project Structure

The project consists of the following main components:
- **data**: Folder containing the provided data.
- **code**: Folder containing the code for data processing, analysis, and modeling.
- **README.md**: Overview and description of the project.

## Code Description

### Data Loading and Merging

The data is loaded from the provided Excel file and merged into a single dataframe using `customerID` as the key.

### Exploratory Data Analysis (EDA)

The relationship between churn and client characteristics is explored using summary statistics and visualizations. Key plots include:
- Count plot for churn
- Count plot for churn by gender
- Box plots for MonthlyCharges and TotalCharges by churn

### Data Cleaning and Preprocessing

The following steps are performed:
- Handling missing values
- Treating outliers
- Addressing class imbalance if necessary

### Feature Engineering

Additional features may be created or transformed if necessary.

### Model Building

A classification model is proposed and fit to predict customer churn. The data is split into training and testing sets to evaluate model performance.

### Model Evaluation

The model's performance is evaluated using appropriate metrics such as accuracy, precision, recall, and F1 score.

## Usage

To reproduce the analysis and model, follow these steps:

1. Ensure you have the required dependencies installed:
    ```bash
    pip install pandas seaborn matplotlib
    ```

2. Run the analysis script:
    ```bash
    python analysis.py
    ```

3. The results, including visualizations and model performance metrics, will be saved in the appropriate output folders.

## Conclusion

This project provides a comprehensive analysis of customer churn for DMResources Limited and proposes a predictive model to help reduce churn and optimize profit. The methodology ensures reproducibility, scalability, and high quality.

