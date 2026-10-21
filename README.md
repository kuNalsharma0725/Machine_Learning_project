# Machine_Learning_project
This project uses machine learning to predict whether a telecom customer is likely to leave the service(**churn**) based on customer information such as tenure, contract type, monthly charges, total charges, and service-related features.    
The project demonstrates a basic end-to-end classification workflow: cleaning a dataset, preparing features, encoding categorical values, training a cllasification model, and collecting customer details to make a prediction.
## Objectives

-   Explore and clean customer data.
-   Prepare categorical and numerical features for machine learning.
-   Train a classification model to predict customer churn.
-   Build an interactive prediction script that accepts customer
    details.
    ## Dataset

The dataset used in the notebook contains customer attributes and a
target column named `Churn`. The screenshots show a cleaned dataset with
**1,000 rows and 11 columns** after removing the `customerID` column and
checking for duplicate rows.
Features shown in the project include:

-   `gender`
-   `SeniorCitizen`
-   `tenure`
-   `PhoneService`
-   `InternetService`
-   `Contract`
-   `PaperlessBilling`
-   `PaymentMethod`
-   `MonthlyCharges`
-   `TotalCharges`
-   `Churn` (target)
-   
## Workflow

1.  **Load the dataset** into a pandas DataFrame.
2.  **Clean the data** by removing the `customerID` column and checking
    for duplicate rows.
3.  **Encode the target** by mapping `Churn` values from `Yes`/`No` to
    `1`/`0`.
4.  **Encode categorical features** with one-hot encoding
    (`pandas.get_dummies`, using `drop_first=True` in the shown
    notebook).
5.  **Train a classification model** using the prepared features and
    target.
7.  **Make predictions** by collecting inputs such as tenure, monthly
    charges, total charges, senior-citizen status, and contract type.
8.  **Align prediction inputs** with the feature columns used during
    training before passing them to the model.
    
   ## Technologies Used
Python
-   pandas
-   NumPy
-   scikit-learn

## Using the Prediction Script
The script asks for these values:

-   **Tenure (months):** how long the customer has been with the
    company.
-   **Monthly charges:** the customer's monthly bill.
-   **Total charges:** the customer's total billed amount.
-   **Senior citizen:** enter `1` for Yes or `0` for No.
-   **Contract type:** enter `0` for month-to-month, `1` for one year,
    or `2` for two years.

  Example inputs from the notebook:

``` text
Tenure: 24
Monthly charges: 65.50
Total charges: 1500
Senior citizen: 0
Contract type: 1
```

These are example inputs only; the prediction depends on the trained
model and preprocessing used in your notebook.
## Results

-   Accuracy: 0.7069
-   Precision
-   Recall
-   F1-score
-   Confusion matrix




