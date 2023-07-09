# Customer Churn Prediction
This project aims to predict customer churn for a telecommunications company. The dataset used in this project contains various features related to customer demographics, usage patterns, and services subscribed. The goal is to build a binary classification model that can accurately predict whether a customer is likely to churn or not.

## Dataset
The dataset used for this project is stored in the file customer_churn.csv. It consists of the following columns:

- Age: The age of the customer
- Number of Dependents: The number of dependents of the customer
- Tenure in Months: The duration of the customer's tenure
- Avg Monthly Long Distance Charges: The average monthly long distance charges
- Total Charges: The total charges incurred by the customer
- Total Refunds: The total refunds given to the customer
- Total Extra Data Charges: The total extra data charges for the customer
- Total Long Distance Charges: The total long distance charges for the customer
- Total Revenue: The total revenue generated from the customer
- Average Charges per Month: The average charges per month for the customer
- Married_Yes: Binary variable indicating whether the customer is married or not (1 = married, 0 = not married)
- Offer_Offer A, Offer_Offer B, Offer_Offer C, Offer_Offer D, Offer_Offer E: Binary variables indicating the offer type subscribed by the customer (1 = subscribed, 0 = not subscribed)
- Internet Service_Yes: Binary variable indicating whether the customer has internet service or not (1 = has internet service, 0 = no internet service)
- Contract_One Year, Contract_Two Year: Binary variables indicating the contract duration (1 = one year/two years, 0 = month-to-month)
- Paperless Billing_Yes: Binary variable indicating whether the customer has opted for paperless billing (1 = opted, 0 = not opted)
- Payment Method_Credit Card, Payment Method_Mailed Check: Binary variables indicating the payment method used by the customer (1 = used, 0 = not used)
- Customer Status_Stayed: Binary variable indicating whether the customer stayed (1 = stayed, 0 = churned)
## Data Preprocessing
Before building the classification model, the dataset underwent several preprocessing steps, including:

- Handling missing values
- Scaling numerical features using StandardScaler
- Encoding categorical features using one-hot encoding
## Model Training and Evaluation
The dataset was split into training and test sets, with 80% of the data used for training and 20% for testing. The following models were trained and evaluated:

- Logistic Regression: A binary classification model using logistic regression algorithm
- Support Vector Machines (SVM): A binary classification model using SVM algorithm
The models were evaluated using various evaluation metrics, including precision, recall, f1-score, and accuracy.

## Hyperparameter Tuning
For the SVM model, hyperparameter tuning was performed using grid search with cross-validation. The following hyperparameters were tuned:

C: The regularization parameter
kernel: The type of kernel function used
gamma: The kernel coefficient for 'rbf', 'poly', and 'sigmoid' kernels
# Conclusion
Based on the evaluation results, the SVM model with the tuned hyperparameters achieved good performance in predicting customer churn. The model demonstrated high precision, recall, and f1-score, indicating its effectiveness in identifying churned customers. The accuracy of the model on the test set was also satisfactory.
