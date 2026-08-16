# Python for Data Science: Healthcare Predictive Analytics Foundations

This repository contains the complete implementation for the **TOPS Python For Data Science Assessment**, focusing on predictive analytics and exploratory data analysis using the UCI Heart Disease dataset.

## 🚀 Overview

The assessment is divided into three core sections, moving from theoretical data science foundations to hands-on clinical data pipelines.

### 📚 Section A: Concept Application
*   **File:** `Section_A_Concept_Application.ipynb`
*   **Description:** Covers foundational data science concepts including:
    *   The difference between `.py` scripts and `.ipynb` Jupyter Notebooks.
    *   Distinguishing between numerical and categorical features in clinical data.
    *   Understanding why target variable data types define the framing of a prediction problem (Classification vs. Regression).
    *   Interpreting correlation values and what they indicate about feature relationships.
    *   The fundamental difference between hardcoded Static Rule-Based Systems and dynamic Data-Driven Machine Learning approaches.

### 💻 Section B: Practical Task
*   **File:** `Section_B_Practical_Task.ipynb`
*   **Description:** Hands-on data engineering and analysis using Pandas and Seaborn:
    *   **Data Ingestion:** Automated pipeline to load the UCI dataset and perform categorical type-casting for clinical variables (`sex`, `cp`, `restecg`).
    *   **Outlier Detection:** Implemented the Interquartile Range (IQR) method to detect and filter statistical anomalies in cholesterol (`chol`) and max heart rate (`thalach`), visualized via Boxplots.
    *   **Multivariate Analysis:** Correlation heatmaps to identify multi-collinearity between clinical features and uncover the strongest predictors of heart disease.
    *   **Feature Engineering:** Created derived features (e.g., 'Age-adjusted Max Heart Rate' and 'Heart Rate Reserve') and normalized numerical data using `StandardScaler` to improve predictive signals.

### 🏆 Section C: Mini Project
*   **Files:** 
    *   `Section_C_Mini_Project.ipynb`
    *   `Section_C_Comparison_Report.md`
    *   `cleaned_heart_disease.csv`
*   **Description:** "Cardiac Risk Stratification and Clinical Decision Support System."
    *   **Data Cleaning:** Pre-processed the Kaggle UCI dataset (normalized headers, handled missing values, binarized targets) and exported the final `cleaned_heart_disease.csv`.
    *   **EDA:** Documented Exploratory Data Analysis comparing age, cholesterol, and heart rates against heart disease presence.
    *   **Feature-Target Interaction:** Generated a focused interaction matrix to isolate key clinical drivers.
    *   **Comparison Report:** A concise, professional breakdown analyzing the pros and cons of utilizing Data Science Predictive Modeling over traditional Static Rule-Based Thresholds in a hospital setting.

---

## 🛠️ How to Run

Ensure you have Python 3 installed along with the required Data Science packages:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

1. Download the [UCI Heart Disease Dataset from Kaggle](https://www.kaggle.com/datasets/ronitf/heart-disease-uci).
2. Place the `heart_disease_uci.csv` file into the root of this repository.
3. Open and run the Jupyter Notebooks sequentially to view the analysis and visual outputs!
