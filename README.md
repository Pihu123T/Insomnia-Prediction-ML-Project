# Insomnia-Prediction-ML-Project
# 💤 Predicting Insomnia Using Machine Learning Classification Models

## 📌 Project Overview

This project focuses on predicting moderate/severe insomnia using machine learning classification algorithms. It explores the relationship between insomnia and different demographic, lifestyle, and health-related factors.

The project uses Python and Scikit-learn to train, evaluate, and compare four classification models to identify which performs best on the given dataset.

**Note:** This is an educational machine learning project based on dataset labels. It is not a medical diagnosis tool.

## 🎯 Project Objective

The main objective is to classify participants into two categories:

- **1 – Moderate/Severe Insomnia:** Participants labelled with moderate or severe insomnia according to the dataset's doctor-opinion label.
- **0 – Other Insomnia Categories:** Participants belonging to all other insomnia categories.

## 📊 Dataset Description

The dataset contains information related to participants' demographic characteristics, lifestyle habits, sleep timings, and health conditions.

Some of the features used include:

- Gender
- Age
- Living Status
- Occupation
- Educational Year
- Marital Status
- Smoking Habits
- Alcohol Consumption
- Place of Education
- University Type
- Sleep Time
- Asthma
- Hypertension
- Heart Disease
- Cardiovascular Disease
- Cancer
- Diabetes
- Doctor's Opinion on Anxiety

## 🛠️ Technologies & Libraries Used

- **Python** – Programming language
- **Jupyter Notebook** – Development environment
- **Pandas** – Data manipulation and cleaning
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine learning algorithms and evaluation

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Loaded the Excel dataset using Pandas.
- Examined dataset structure, columns, and data types.
- Identified missing values and duplicate participant IDs.

### 2. Data Cleaning and Preprocessing
- Removed duplicate participant IDs.
- Handled missing values.
- Standardized text values by removing extra spaces and converting text to lowercase.
- Selected relevant columns for the project.

### 3. Feature Engineering

Created additional features to support classification:

- **DiseaseCount:** Total number of reported chronic diseases.
- **LateSleeper:** Identifies participants who sleep after midnight.
- **RiskyHabits:** Counts reported smoking and alcohol habits.

### 4. Exploratory Data Analysis (EDA)

Multiple visualizations were created to understand the dataset and identify patterns.

Visualizations include:

- Insomnia Class Distribution (Count Plot and Pie Chart)
- Moderate/Severe Insomnia Rate by Age Group
- Moderate/Severe Insomnia Rate by Sleep Time
- Percentage Distribution of Participants by Sleep Time
- Insomnia Rate Across Different Anxiety Levels
- Disease Count vs. Risky Habits (Scatter Plot)
- Distribution of Reported Diseases by Insomnia Class (Box Plot)

### 5. Train-Test Split

- Training Data: 70%
- Testing Data: 30%
- Random State: 42
- Stratified splitting was used to maintain class proportions.

Feature scaling was applied for models such as KNN and SVM.

## 🤖 Machine Learning Models

Four classification algorithms were implemented and evaluated separately.

| Model | Algorithm |
|---|---|
| Model 1 | K-Nearest Neighbors (KNN) |
| Model 2 | Gaussian Naive Bayes |
| Model 3 | Decision Tree |
| Model 4 | Support Vector Machine (SVM) |

### Model Evaluation Metrics

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

## 📈 Model Performance Comparison

The following test accuracy results were obtained:

| Classification Model | Accuracy |
|---|---:|
| KNN | 93.64% |
| Naive Bayes | 92.14% |
| Decision Tree | 94.97% |
| SVM | 94.11% |

**Best Performing Model: Decision Tree**

The Decision Tree achieved the highest test accuracy of **94.97%** among the four implemented models.

Other evaluation metrics were also considered because accuracy alone does not provide a complete picture of classification performance.

## 📉 Additional Model Visualizations

The project also includes:

- Confusion Matrix for KNN
- Confusion Matrix for Naive Bayes
- Confusion Matrix for Decision Tree
- Confusion Matrix for SVM
- Accuracy Comparison of All Four Models
- Decision Tree Feature Importance
- SVM Decision Boundary Visualization
- Decision Tree Structure Visualization

## 📁 Project Structure

```text
Insomnia-Prediction-ML-Project/
│
├── Insomnia_Prediction.ipynb
│
├── README.md
│
└── Onidra_Raw_Dataset.xlsx
```

*The dataset is listed for reference. Include it in the repository only if you have permission to share it and it contains no identifiable or sensitive participant information.*

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Open Anaconda Navigator.
3. Launch Jupyter Notebook.
4. Open `Insomnia_Prediction.ipynb`.
5. Ensure the required Python libraries are installed.
6. Keep the dataset in the same folder as the notebook, if you have authorized access to it.
7. Run the notebook cells sequentially.

### Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Data cleaning and preprocessing.
- Feature engineering.
- Exploratory Data Analysis.
- Implementing multiple classification algorithms.
- Training and evaluating machine learning models.
- Comparing model performance using different evaluation metrics.
- Understanding confusion matrices and classification reports.
- Visualizing model decisions and feature importance.

## ⚠️ Disclaimer

This project is developed strictly for educational and academic purposes. The predictions are based on the labels available in the dataset and should not be interpreted as medical advice, clinical assessment, or a diagnostic result.

---

**Thank you for visiting my project!** 😊

Feel free to explore the notebook and its implementation.
