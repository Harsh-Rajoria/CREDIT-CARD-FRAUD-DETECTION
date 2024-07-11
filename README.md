# CREDIT-CARD-FRAUD-DETECTION
This my 5th Project on DataScience
      CREDIT CARD FRAUD DETECTION
1. Build a machine learning model to identify fraudulent credit card
transactions.
2. Preprocess and normalize the transaction data, handle class
imbalance issues, and split the dataset into training and testing sets.
3. Train a classification algorithm, such as logistic regression or random
forests, to classify transactions as fraudulent or genuine.
4. Evaluate the model's performance using metrics like precision, recall,
and F1-score, and consider techniques like oversampling or
undersampling for improving results.

Dataset:-https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Steps in the Code:

1. **Data Loading and Exploration**:
   - Loads the credit card transactions dataset (`credit_card_transactions.csv`).
   - Checks the class balance between fraudulent and genuine transactions.

2. **Data Preprocessing**:
   - Separates features (`X`) and target variable (`y`).
   - Normalizes the features using `StandardScaler` to scale them to zero mean and unit variance.

3. **Handling Class Imbalance**:
   - Uses `SMOTE` (Synthetic Minority Over-sampling Technique) to oversample the minority class (fraudulent transactions) to balance the dataset.

4. **Model Training**:
   - Initializes a `LogisticRegression` model.
   - Trains the model on the resampled training data (`X_train_resampled`, `y_train_resampled`).

5. **Model Evaluation**:
   - Makes predictions on the test set (`X_test`).
   - Evaluates the model's performance using `classification_report`, which includes metrics like precision, recall, and F1-score.
