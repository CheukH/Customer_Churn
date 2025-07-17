# Analysis of Decision Tree and Naïve Bayes Models for Customer Churn Prediction in Imbalanced Class Distribution

This project aims to predict telecom customer churn using Decision Tree and Naive Bayes classifiers. The objective is to identify customers that are likely to leave the service and support data-driven retention strategies.
The dataset contains 3,333 observations with 21 features as described below:

- State: Customer’s state.
- Account Length: Integer number showing the duration of activity for the customer account.
- Area Code: Area code of the customer.
- Phone Number: Phone number of the customer.
- Inter Plan: Binary indicator showing whether the customer has an international calling plan.
- VoiceMail Plan: Indicator of voicemail plan.
- No of Vmail Mesgs: The number of voicemail messages.
- Total Day Min: The number of minutes the customer used the service during daytime (continuous quantitative data type).
- Total Day Calls: Discrete attribute indicating the total number of calls during daytime.
- Total Day Charge: Charges for using the service during daytime (continuous data type).
- Total Evening Min: The number of minutes the customer used the service during evening time.
- Total Evening Calls: The number of calls during evening time.
- Total Evening Charge: Charges for using the service during evening time.
- Total Night Min: Number of minutes the customer used the service during night time.
- Total Night Calls: The number of calls during night time.
- Total Night Charge: Charges for using the service during night time.
- Total Int Min: Number of minutes the customer used the service to make international calls.
- Total Int Calls: The number of international calls.
- Total Int Charge: Charges for international calls.
- No of Calls Customer Service: The number of calls to customer support service.
- Churn: Class attribute with binary values (True for churn and False for not churn).

Due to a significant class imbalance, model performance was evaluated using metrics focused on the F1-score of the minority (churn) class.

Both models were trained using a Train-Validation-Test split (60/20/20). Irrelevant features were removed, and categorical variables were processed using One-Hot Encoding.

Models were fine-tuned using hyperparameter search, and the decision threshold was adjusted to improve performance on the churn class.

Final results show that the Decision Tree consistently outperformed Naive Bayes, especially in identifying churn cases, and is recommended for deployment.
