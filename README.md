# SPAMML
## 📖 Project Overview

This project focuses on building a machine learning model that detects **spam SMS messages** using a Naive Bayes classifier.  
By leveraging TF-IDF vectorization and simple yet powerful preprocessing techniques, the model classifies each message as either:

- **Ham** (legitimate message) or
- **Spam** (unwanted message)

The final trained model achieves high accuracy, making it practical for real-world deployment in communication filtering systems.

---

## 📂 Dataset Information

- **Dataset Source**: [Kaggle - SMS Spam Collection Dataset](https://www.kaggle.com/datasets/kartik2112/fraud-detection)
- **Format**: CSV file containing text messages and their labels.
- **Classes**: 
  - `ham` — legitimate message
  - `spam` — unwanted/spam message
- **Number of Samples**: Approximately 5,500 SMS messages.

**Important Note**: Only the necessary columns were selected, and labels were encoded (`ham: 0`, `spam: 1`) for machine learning compatibility.

---

## 🛠 Project Workflow

### 1. Data Preprocessing
- Selected only required columns (`label`, `message`).
- Converted the labels into binary values (0 or 1).
- Applied text cleaning:
  - Lowercasing all text.
  - Removing numbers and punctuation.
  - Removing unnecessary whitespace.

### 2. Feature Engineering
- Utilized **TF-IDF (Term Frequency - Inverse Document Frequency)** vectorization to transform text messages into numerical features.
- Ignored common English stopwords to focus on meaningful words.

### 3. Model Training
- Used **Multinomial Naive Bayes**, a preferred model for text classification tasks.
- The model was trained on the TF-IDF-transformed features.

### 4. Model Evaluation
- Splitting the dataset: 80% for training, 20% for testing.
- Evaluated the model based on:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1 Score**
  - **ROC-AUC Score**
- Confusion Matrix was also visualized for better error analysis.

### 5. Testing
- Conducted testing with a sample real-world spam message to validate model behavior.

---

## 🚀 How to Run This Project

### Prerequisites
Make sure Python and the following libraries are installed:
pip install pandas numpy scikit-learn matplotlib

Then follow these steps
1. clone this repository
2.Add the dataset
3. Run the Notebook.

#Author PraveenKumar G
