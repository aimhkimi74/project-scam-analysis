# Developing a Predictive Model to Determine Scam Likelihood: A Case Study on the General Population 🛡️

---

## 📖 Overview
This project investigates the critical factors influencing scam vulnerability in contemporary society. Developed as a Big Data and Machine Learning project for **CSC649 (Special Topic in Computer Science)** at **Universiti Teknologi MARA (UiTM)**, this research utilizes predictive modeling to identify behavioral patterns and socioeconomic conditions that increase scam susceptibility.

---

## 🏆 Key Performance Metrics
The model was rigorously tested using multiple algorithms and 4-fold cross-validation to ensure high reliability.

* **Best Performing Model:** Random Forest Classifier.
* **Testing Accuracy:** Achieved a high **91.17% accuracy** on unseen data.
* **Training Accuracy:** 100%, indicating a perfect fit on the training dataset.
* **Feature Optimization:** Maintained a strong **85.55% testing accuracy** even when reduced to the top 5 most critical features.

---

## 🔍 Feature Importance Insights
Through feature selection experiments, we identified the top 5 predictors most indicative of an individual's vulnerability to online scams:

1. **Habit of reading reviews before buying** (Highest Impact).
2. **Frequency of sharing personal information online**.
3. **Downloads from untrusted sources**.
4. **Maximum amount spent in a single transaction**.
5. **Average daily online hours**.

---

## 📊 Methodology
* **Data Collection:** Analyzed **500 responses** from a structured survey distributed over a 50-day period.
* **Data Preprocessing:**
    * Renamed 19 features for clarity and removed non-contributing columns like timestamps.
    * Applied **Label Encoding** to transform qualitative attributes into numerical formats for machine learning processing.
    * Addressed class imbalance through **upsampling** of the minority class to improve fraud detection capabilities.
* **Model Tuning:** Explored over **200 hyperparameter combinations** during the cross-validation phase to identify the optimal configuration.

---

## 📂 Project Structure
```text
project-scam-analysis/
│
├── data/
│   ├── scam_survey_responses.csv      # Original raw survey data
│   └── cleaned_scam_data.csv          # Preprocessed and balanced dataset
├── notebooks/
│   ├── 01_Data_Exploration_Analysis.ipynb # Categorical & Numerical visualizations
│   ├── 02_Data_Preprocessing.ipynb        # Cleaning, encoding, and upsampling
│   └── 03_Predictive_Modeling_RF.ipynb    # Random Forest training & Feature Selection
├── docs/
│   └── Technical_Report.pdf           # Full technical documentation
├── requirements.txt                   # Project dependencies
└── README.md                          # Project documentation
```
---

## 📋 Data Dictionary

The dataset contains 20 features capturing demographic and behavioral data. Below is a description of the key variables:

| Feature | Description |
| :--- | :--- |
| **Scammed** | Target Variable (1: Has been scammed, 0: Has not) |
| **Age_Group** | Categorical age ranges of respondents |
| **Income** | Monthly income level in local currency (MYR) |
| **Daily_Online_Hours** | Average time spent on the internet per day |
| **Stranger_Interactions** | Frequency of interacting with unknown individuals online |
| **Monthly_Online_Transactions** | Number of digital purchases made per month |
| **Shares_Personal_Info** | Whether the user tends to share private data online |
| **Downloads_From_Untrusted_Sources** | Frequency of downloading files from non-verified sites |
| **Reads_Reviews_Before_Buying** | Consumer behavior regarding product research |
| **Max_Single_Transaction_Spend** | The highest amount ever spent in one online purchase |

---
## 🛠️ Tech Stack
Language: Python 3.10

* Libraries: Pandas, NumPy (Data Manipulation)
* Visualization: Matplotlib, Seaborn
* Machine Learning: Scikit-Learn (Random Forest, K-Fold, Label Encoding)
---

## 👥 The Team
This project was a collaborative effort by group members from UiTM:

* Muhammad Ariff 
* Muhamad Ikhwan Dannial
* Muhammad Amirul Mifzal
* Muhammad Akid Danial
* Muhammad Aiman Hakimi
---
## 📝 License & Citation
* Completed on 3 February 2025. This project is intended for educational and portfolio purposes. Please credit the original authors and UiTM when referencing this work.