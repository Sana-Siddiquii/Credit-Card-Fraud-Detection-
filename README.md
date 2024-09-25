
# **Credit Card Fraud Detection Project**

This project involves the development of a machine learning model to detect fraudulent credit card transactions. The primary tasks undertaken include:

### 1. **Data Preprocessing**:
   - **Handling Missing Values**: Identified missing data and filled numerical columns with median values to prevent data loss and maintain model accuracy.
   - **Categorical Variable Encoding**: Transformed categorical variables such as "Merchant", "Location", and "Card Type" into numerical values using label encoding.
   - **Target Variable Preparation**: Converted the target variable, "Is Fraudulent", into a binary format (1 for fraud, 0 for non-fraud), ensuring the data was ready for classification modeling.

### 2. **Exploratory Data Analysis (EDA)**:
   - **Transaction Distribution**: Analyzed the distribution of legitimate versus fraudulent transactions, revealing a significant class imbalance (legitimate transactions vastly outnumbered fraudulent ones).
   - **Transaction Amount Analysis**: Studied the range of transaction amounts, observing that fraudulent and legitimate transactions showed similar distributions, indicating that transaction amount alone could not be used to detect fraud.
   - **Pattern Identification**: Identified key patterns and trends in the data to inform the feature engineering and modeling process.

### 3. **Feature Engineering**:
   - **Time-Based Features**: Extracted the transaction hour from the transaction date to capture temporal patterns in fraudulent behavior.
   - **Customer Behavior**: Calculated transaction frequency per customer to identify abnormal behaviors indicative of fraud.
   - **Enhanced Predictive Features**: Engineered new features that improved the model's ability to detect subtle fraud patterns.

### 4. **Model Development**:
   - **Random Forest Classifier**: Selected the Random Forest algorithm for its robustness in handling imbalanced datasets and ability to capture non-linear relationships.
   - **Train-Test Split**: Divided the dataset into 70% training and 30% testing sets to validate model performance.
   - **Model Training**: Trained the Random Forest model using the training dataset, optimizing hyperparameters to balance precision and recall.
   - **Addressing Class Imbalance**: Implemented techniques within the model to handle the class imbalance between legitimate and fraudulent transactions.

### 5. **Model Evaluation**:
   - **Accuracy**: Achieved high accuracy in correctly classifying both legitimate and fraudulent transactions.
   - **Precision & Recall**: High precision meant that the model was effective in predicting fraud with minimal false positives, while recall ensured a good detection rate for actual fraud cases.
   - **AUC-ROC Curve**: The model achieved a high area under the ROC curve (AUC), demonstrating strong discriminatory ability between fraudulent and non-fraudulent transactions.
   - **Confusion Matrix**: Analyzed the confusion matrix to understand where the model made errors, identifying opportunities for further optimization.

### 6. **Recommendations & Future Work**:
   - **Continuous Model Updates**: Proposed a system for continuous learning, regularly updating the model with new data to adapt to evolving fraud patterns.
   - **Real-Time Fraud Detection**: Recommended deploying the model in a real-time environment to enable instant detection of suspicious transactions.
   - **Handling Class Imbalance**: Suggested the use of SMOTE (Synthetic Minority Oversampling Technique) to mitigate the impact of class imbalance on model performance.
   - **Behavioral Features**: Recommended incorporating additional behavioral features such as location consistency and customer spending patterns for more accurate fraud detection.

---

