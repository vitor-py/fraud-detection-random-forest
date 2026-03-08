#  Credit Card Fraud Detection

A machine learning project that detects fraudulent credit card transactions using a Random Forest classifier.

The model analyzes behavioral and transactional features such as transaction distance, purchase value relative to a customer's typical spending, and transaction method to classify operations as fraudulent or legitimate.

---

#  Project Overview

Financial fraud detection is an important application of machine learning. In this project, a classification model was trained to identify suspicious transactions based on behavioral patterns.

The model evaluates several indicators, including:

- distance from the customer's home
- distance from the previous transaction
- purchase amount relative to the customer's median spending
- whether the retailer is frequently used
- chip and PIN usage
- online transaction status

These features help identify unusual transaction behavior that may indicate fraud.

---

#  Model

The model was trained using:

- Random Forest classifier
- Stratified train/test split
- Feature importance analysis

Random Forest was chosen because it performs well on tabular data and can capture non-linear relationships between features.

---

# 📈 Results

The model achieved strong performance on the test dataset:

- High accuracy
- Strong precision and recall
- Effective identification of fraudulent patterns present in the dataset

Feature importance analysis showed that the most influential variables were:

- ratio_to_median_purchase_price
- distance_from_home
- online_order

These variables contributed most to the model's fraud detection capability.

---

# ⚠️ Observations

During testing, the model performed very well when fraudulent transactions followed clear patterns present in the dataset.

However, when synthetic transactions were created that closely resembled legitimate behavior (for example purchases close to home with normal spending values), the model sometimes classified them as legitimate.

This highlights a common limitation of supervised learning models: they can only learn patterns present in the training data.

---
