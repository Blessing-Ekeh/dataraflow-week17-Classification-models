# Week 17 - Datasets Dictionary

Information on all the datasets required for completing the Week 17 assignments on Classification Algorithms (K-Nearest Neighbors, Support Vector Machines, and Naive Bayes).

## Folder Structure

```
Week-17 (Classification-1)/
│
├── Task-Datasets/
│   ├── task1_knn_customer_data.csv
│   ├── task2_svm_classification_data.csv
│   └── task3_naive_bayes_data.csv
│
├── Assignment-Dataset/
│   ├── assignment1_product_recommendation.csv
│   ├── assignment2_medical_diagnosis.csv
│   └── assignment3_classifier_comparison.csv
│
└── Assessment-Dataset/
    └── loan_approval_prediction.csv
```


## Task Datasets

### 1. task1_knn_customer_data.csv
**Purpose**: Practice implementing K-Nearest Neighbors classification for customer purchase prediction

**Columns**:
- `Customer_ID` (numeric): Unique customer identifier
- `Gender` (categorical): Male or Female
- `Age` (numeric): Customer age (18-65)
- `Annual_Salary` (numeric): Annual salary in dollars ($15,000-$150,000)
- `Purchased` (binary): Whether customer purchased the product (0=No, 1=Yes)

**Records**: 100 rows  
**Pattern**: Purchase behavior influenced by age and salary combination
**Use Case**: Test different K values and understand distance-based classification

---

### 2. task2_svm_classification_data.csv
**Purpose**: Practice Support Vector Machine classification with different kernels

**Columns**:
- `Feature1` (numeric): First feature dimension (-5 to 5)
- `Feature2` (numeric): Second feature dimension (-5 to 5)
- `Class` (binary): Target class (0 or 1)

**Records**: 150 rows  
**Pattern**: Non-linearly separable data ideal for kernel SVM
**Use Case**: Compare linear vs RBF kernel performance

---

### 3. task3_naive_bayes_data.csv
**Purpose**: Implement Gaussian Naive Bayes for email classification

**Columns**:
- `Email_ID` (numeric): Unique email identifier
- `Word_Count` (numeric): Total words in email (10-500)
- `Link_Count` (numeric): Number of hyperlinks (0-20)
- `Uppercase_Ratio` (numeric): Ratio of uppercase characters (0.0-0.5)
- `Special_Char_Count` (numeric): Count of special characters (0-50)
- `Contains_Urgent` (binary): Contains urgent/alert words (0 or 1)
- `Is_Spam` (binary): Whether email is spam (0=Not Spam, 1=Spam)

**Records**: 120 rows  
**Pattern**: Spam emails tend to have more links, uppercase, and special characters
**Use Case**: Demonstrate probabilistic classification with Naive Bayes

---

## Assignment Datasets

### 1. assignment1_product_recommendation.csv
**Purpose**: Advanced KNN implementation with feature scaling and K optimization

**Columns**:
- `Customer_ID` (numeric): Unique identifier
- `Age` (numeric): Customer age (18-70)
- `Annual_Income` (numeric): Annual income in thousands ($15K-$200K)
- `Spending_Score` (numeric): Customer spending score (1-100)
- `Purchase_Frequency` (numeric): Monthly purchase frequency (0-30)
- `Website_Visit_Duration` (numeric): Average visit duration in minutes (1-60)
- `Product_Category_Preference` (categorical): Electronics, Fashion, Home, Sports
- `Will_Buy_Premium` (binary): Will purchase premium product (0=No, 1=Yes)

**Records**: 250 rows  
**Class Balance**: ~65% No, ~35% Yes

---

### 2. assignment2_medical_diagnosis.csv
**Purpose**: SVM classification for medical diagnosis with comprehensive evaluation

**Columns**:
- `Patient_ID` (numeric): Unique patient identifier
- `Age` (numeric): Patient age (20-80)
- `BMI` (numeric): Body Mass Index (15-45)
- `Blood_Pressure` (numeric): Systolic blood pressure (90-200)
- `Glucose_Level` (numeric): Fasting glucose level (70-250)
- `Cholesterol` (numeric): Total cholesterol level (120-350)
- `Heart_Rate` (numeric): Resting heart rate (50-120)
- `Family_History` (binary): Family history of disease (0=No, 1=Yes)
- `Smoking_Status` (categorical): Never, Former, Current
- `Diagnosis` (binary): Disease diagnosis (0=Negative, 1=Positive)

**Records**: 300 rows  
**Class Balance**: ~70% Negative, ~30% Positive
**Complexity**: Requires proper preprocessing and kernel selection

---

### 3. assignment3_classifier_comparison.csv
**Purpose**: Comprehensive comparison of KNN, SVM, and Naive Bayes on same dataset

**Columns**:
- `Sample_ID` (numeric): Unique identifier
- `Feature_A` (numeric): First feature (0-100)
- `Feature_B` (numeric): Second feature (0-100)
- `Feature_C` (numeric): Third feature (0-100)
- `Feature_D` (numeric): Fourth feature (0-100)
- `Categorical_Feature` (categorical): Type_1, Type_2, Type_3
- `Target_Class` (categorical): Class_A, Class_B, Class_C (Multi-class)

**Records**: 350 rows  
**Class Distribution**: Class_A (40%), Class_B (35%), Class_C (25%)
**Use Case**: Compare all three classifiers on multi-class problem

---

## Assessment Dataset

### loan_approval_prediction.csv
**Purpose**: End-to-end classification project using KNN, SVM, and Naive Bayes

**Columns**:
- `Application_ID` (numeric): Unique application identifier
- `Gender` (categorical): Male, Female
- `Married` (categorical): Yes, No
- `Dependents` (numeric): Number of dependents (0-4)
- `Education` (categorical): Graduate, Not Graduate
- `Self_Employed` (categorical): Yes, No
- `Applicant_Income` (numeric): Monthly income ($1,000-$80,000)
- `Coapplicant_Income` (numeric): Co-applicant income ($0-$40,000)
- `Loan_Amount` (numeric): Requested loan amount ($10K-$700K)
- `Loan_Term` (numeric): Loan term in months (12-480)
- `Credit_History` (binary): Credit history meets guidelines (0=No, 1=Yes)
- `Property_Area` (categorical): Urban, Semiurban, Rural
- `Previous_Loan_Status` (categorical): None, Paid, Defaulted
- `Employment_Years` (numeric): Years at current job (0-40)
- `Age` (numeric): Applicant age (21-65)
- `Loan_Approved` (binary): Loan approval status (0=Rejected, 1=Approved)

**Records**: 500 rows  
**Class Distribution**: Approved (~68%), Rejected (~32%)

**Complexity**: Advanced - requires integration of:
- Feature preprocessing (encoding categorical variables)
- Feature scaling (for KNN and SVM)
- Multiple classifier implementation
- Comprehensive evaluation metrics
- Business interpretation

---

## Data Quality Notes

### Key Concepts Demonstrated
| Dataset | Key Concept |
|---------|-------------|
| Task 1 (KNN) | Distance-based classification, K selection |
| Task 2 (SVM) | Kernel selection, margin maximization |
| Task 3 (Naive Bayes) | Probabilistic classification, feature independence |
| Assignment 1 | KNN optimization, feature scaling importance |
| Assignment 2 | SVM kernels, medical classification ethics |
| Assignment 3 | Multi-class comparison, algorithm selection |
| Assessment | End-to-end pipeline, business recommendations |

---

**Note**: Refer to this Data Dictionary when working on Week 17 assignments.
