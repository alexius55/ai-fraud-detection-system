# AI Fraud Detection System

Machine learning and deep learning system for detecting fraudulent financial transactions using the **UCI Credit Card dataset**.

---

## Project Overview

This project develops an artificial intelligence–based fraud detection system capable of identifying suspicious financial transactions. The system compares traditional machine learning and deep learning models while addressing common challenges in fraud datasets such as **class imbalance** and **high dimensionality**.

The project also includes a **Flask-based web application** that allows users to input transaction data and receive a fraud prediction in real time.

---

## Dataset

**UCI Credit Card Default Dataset**

- 30,000 credit card records
- 25 financial and demographic features
- Binary classification:
  - `0` → legitimate transaction
  - `1` → fraudulent/default transaction

Dataset includes variables such as:

- Credit limit
- Payment history
- Bill amounts
- Previous payments
- Demographic attributes

---

## Machine Learning Models

The following models were implemented and compared:

- **Residual Neural Network (ResNet)**
- **Support Vector Machine with Grid Search (SVM-GS)**
- **Adaptive Boosting (AdaBoost)**

These models were evaluated using multiple classification metrics to ensure robust fraud detection performance.

---

## Data Processing Techniques

To improve model performance and address challenges in financial datasets, several preprocessing techniques were applied.

### Feature Engineering

- Principal Component Analysis (**PCA**)
- Dwarf Mongoose Optimization (**DMO**)

### Class Imbalance Handling

- Synthetic Minority Oversampling Technique (**SMOTE**)
- Hybrid method **SMOTE-ENN**

These methods help improve the model's ability to detect rare fraudulent transactions.

---

## Best Model Performance

| Model | Accuracy |
|------|------|
| ResNet | **88.5%** |
| SVM | 85.6% |
| AdaBoost | 82.2% |

The **DMO + SMOTE-ENN pipeline** significantly improved detection accuracy compared to the baseline PCA + SMOTE pipeline.

---

## Web Application

A **Flask-based web application** was developed to demonstrate real-time fraud detection.

Features include:

- User input of transaction attributes
- Fraud prediction output
- Probability score
- Timestamp of prediction

This demonstrates the practical deployment of the fraud detection model.

---

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- NumPy
- Flask
- HTML
- CSS
- JavaScript

---

## Project Structure

```
ai-fraud-detection-system
│
├── fraud_detection_model.ipynb
├── fdetection_model.ipynb
├── banker_run.ipynb
├── dmo_credit_card.ipynb
├── scaler.pkl
├── fd.h5
├── requirements.txt
└── UCI_Credit_Card.csv
```

---

## Future Improvements

Possible improvements for future research include:

- Cost-sensitive fraud detection
- Real-time streaming transaction monitoring
- Concept drift detection
- Explainable AI using SHAP or LIME
- Deployment in financial production systems

---

## Example Prediction

The model can analyse transaction data and determine whether a financial transaction is likely to be fraudulent.

Example output:

Prediction: Fraud  
Probability: 0.87

This demonstrates how machine learning models can assist financial institutions in detecting suspicious transactions in real time.

---

## Author

**Alexius-Mitchell Adai Ohiani**

MSc Cyber Security  
Manchester Metropolitan University
