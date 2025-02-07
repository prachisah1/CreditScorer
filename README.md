# Credit Scoring Risk Model

## Overview
This project develops a **Credit Scoring Risk Model** using **Logistic Regression** to predict loan default probability. The model processes financial data, trains on it, and evaluates its accuracy.

## Key Features
- **Data Preprocessing**: Handles missing values, normalizes data.
- **Train-Test Split**: 80% training, 20% testing.
- **Model Training**: Logistic Regression classifier.
- **Evaluation**: Confusion matrix, accuracy score.
- **Model Exporting**: Saves classifier and scaler for reuse.
- **Prediction Output**: Generates a report of probabilities and outcomes.

## Technologies Used
- **Python, Pandas, NumPy** (Data Processing)
- **Scikit-Learn** (Machine Learning)
- **Joblib** (Model Serialization)
- **Google Colab & Google Drive** (Execution & Storage)

## Dataset
- Stored in Google Drive: `a_Dataset_CreditScoring.xlsx`
- Features include financial indicators, excluding `ID`.
- **Target Variable (`TARGET`)**:
  - `0`: Good Loan
  - `1`: Bad Loan

## Workflow
1. **Import Libraries**
2. **Load & Prepare Data**
   - Read dataset from Google Drive
   - Drop `ID` column
   - Handle missing values
   - Split into features (`X`) and target (`y`)
3. **Train-Test Split & Normalization**
   - 80% training, 20% testing
   - StandardScaler for normalization
   - Save scaler with `joblib`
4. **Model Training & Exporting**
   - Train **Logistic Regression**
   - Save trained model with `joblib`
5. **Evaluation & Predictions**
   - Compute **Confusion Matrix** & **Accuracy Score**
   - Predict loan default probabilities
   - Save results as `c1_Model_Prediction.xlsx`

## Setup & Execution
1. Open **Google Colab**.
2. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
3. Upload dataset and run the notebook.

## Output Files
- **Trained Model**: `f1_Classifier_CreditScoring`
- **Scaler File**: `f2_Normalisation_CreditScoring`
- **Predictions Report**: `c1_Model_Prediction.xlsx`

