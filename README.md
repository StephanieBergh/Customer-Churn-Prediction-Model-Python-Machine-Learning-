# Customer Churn Prediction (Telecom Dataset)

A machine learning project that predicts customer churn using real-world telecom data. The goal is to identify customers likely to leave and compare model performance between Logistic Regression and Random Forest classifiers.

---

## Objective

To analyze customer behavior and build predictive models that identify churn risk, enabling businesses to improve customer retention strategies.

---

## Dataset

- Telco Customer Churn dataset
- Contains customer demographics, account information, and service usage
- Target variable: `Churn` (Yes/No)

---

## Workflow

### 1. Data Preprocessing
- Converted numerical columns
- Handled missing values
- Encoded categorical variables using one-hot encoding
- Dropped irrelevant features (e.g., customerID)

### 2. Exploratory Data Analysis (EDA)
- Correlation heatmap
- Tenure distribution analysis
- Monthly vs Total charges relationship
- Churn vs tenure comparison

### 3. Feature Engineering
- One-hot encoding of categorical variables
- Feature selection using:
  - Logistic regression coefficients
  - Permutation feature importance

---

## Models Used

### Logistic Regression
- Scaled features using MinMaxScaler
- Used as baseline model
- Evaluated using accuracy, precision, recall

### Random Forest Classifier
- Ensemble model with 2000 estimators
- Used permutation feature importance
- Evaluated with OOB score and classification metrics

---

## Results

### Logistic Regression
- Accuracy: ~XX
- Precision: 62%
- Recall: 52%
- Struggles to detect churners (high false negatives)

### Random Forest
- Accuracy: ~XX
- Precision: 74%
- Recall: 71%
- Better at identifying churn customers

---

## Key Insights

- Customers with low tenure are more likely to churn
- Monthly charges strongly correlate with total charges
- Random Forest significantly outperforms Logistic Regression for this dataset
- Feature selection improves interpretability

---

## Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

---

## How to Run

### Prerequisites

Make sure Python 3 is installed on your system.

You can verify your installation by running:

```bash
python --version
```

### Installation

1. Clone the repository:

```bash
git clone https://github.com/StephanieBergh/Task_Manager.git
```

2. Navigate to the project folder:

```bash
cd Task_Manager
```

3. Install required packages:

```bash
pip install tabulate
```

### Running the Application

Run the program from the terminal:

```bash
python task_manager.py
```

## Author

** Stephanie Bergh **  
Data Analyst
