# BA_customer_booking

🧠 Customer Booking Prediction Using Logistic Regression
This project uses Logistic Regression to predict whether a customer will complete a booking based on a dataset of customer behavior. The goal is not only to predict the outcome but also to understand how each variable contributes to the prediction.


📁 Dataset
The dataset (customer_booking_ba.csv) contains 50,000 samples with both categorical and numeric features. The target variable is booking_complete:
1 = Customer completed a booking
0 = Customer did not complete a booking


⚙️ Tools & Libraries
pandas for data manipulation
scikit-learn for machine learning pipeline and modeling
matplotlib and seaborn for visualization


🚀 Steps in the Code
Data Preparation:
  Split features (X) and target (y)
  Identify categorical and numeric columns
  One-hot encode categorical variables using ColumnTransformer

Modeling:
    Use LogisticRegression with a pipeline for preprocessing + training
    Split data into 80% train / 20% test

Evaluation Metrics:
  Accuracy Score
  Classification Report
  Confusion Matrix
  Predicted probability distribution plot


📊 Model Evaluation Results
✅ Accuracy: 0.8526
📋 Classification Report:
              precision    recall  f1-score   support

           0       0.86      0.99      0.92      8520
           1       0.51      0.08      0.13      1480

    accuracy                           0.85     10000
   macro avg       0.69      0.53      0.53     10000
weighted avg       0.81      0.85      0.80     10000


🧾 Confusion Matrix:
True Negatives (TN): 8433
False Positives (FP): 87
False Negatives (FN): 1360
True Positives (TP): 120
The model performs well for predicting the majority class (No Booking), but struggles with detecting bookings (minority class), highlighting class imbalance.
