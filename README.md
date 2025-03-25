Introduction
In this project, I will implement credit card fraud detection using different machine learning models and techniques to achieve maximum accuracy. The focus will be on writing clean, efficient, and concise code. If you find my work helpful, please consider upvoting.

Imagine receiving a call from your bank, where a customer service representative informs you that your credit card is about to expire in a week. You check your card details and find that it will expire in eight days. To renew your membership, the representative asks for details like your card number, expiry date, and CVV. Would you share these details?

In such situations, caution is essential, as sharing sensitive information could lead to unauthorized access to your account.

Despite a 51% growth in digital transactions in India (2018–2019), security concerns remain high. Fraudulent activities have surged, with over 52,304 cases of credit/debit card fraud reported in FY 2019 alone. As financial fraud continues to rise, detecting these fraudulent transactions in real time is crucial for protecting consumers and banks. Machine learning can play a vital role in addressing this challenge.

Objective
The primary goal of this project is to detect fraudulent credit card transactions using machine learning techniques. Given the increasing number of digital transactions and rising fraud cases, it is crucial to develop an efficient, accurate, and scalable fraud detection system.

Problem Statement
Credit card fraud is a growing concern due to the rise in digital transactions. Traditional methods struggle to detect fraud effectively, making machine learning essential. The challenge lies in handling imbalanced data and minimizing false predictions. This project aims to develop models that accurately detect fraudulent transactions. The goal is to enhance security while reducing financial losses.

Data Description
we load the data and observe that it contains 31 columns, including 28 important features labeled from V1 to V28, which represent anonymized account-related information. We will retain these features and use the Class column, which contains 0 for normal transactions and 1 for fraudulent transactions, as the target variable
Fraud detection model using logistic regression has been successfully implemented with the following conclusions:

Class Imbalance Handling
The original dataset was highly imbalanced, which could have negatively impacted model performance.
SMOTE was applied to oversample the minority (fraudulent) class, improving the model’s ability to detect fraud.

Feature Engineering
Hour-based analysis was introduced by converting the Time column into an hourly feature.
Transaction Frequency per Hour was computed to capture patterns in transaction behavior.
Log transformation was applied to the Amount column to reduce skewness and improve model performance.

Model Performance
Classification Report shows the effectiveness of the model in identifying fraudulent transactions.

Potential Enhancements.
Fine-tune SMOTE parameters to avoid overfitting and ensure better generalization.
Perform hyperparameter tuning on logistic regression to optimize its performance.

My fraud detection model achieved the following results:
Training Accuracy: 98.64%
Test Accuracy: 98.65%
