# Analysis of the CICIDS 2017 Dataset for Intrusion Detection Research ( Group 15 ) 
Our project in kaggle 
link : https://www.kaggle.com/code/mohammedrahmaniii/person2-datapreprocessing-final

This repository contains our data mining project analyzing the CICIDS 2017 dataset for intrusion detection research.

## Project Overview

This project analyzes the CICIDS 2017 dataset for intrusion detection research using data mining techniques.

## Dataset Overview

The **CICIDS 2017** dataset was developed by the Canadian Institute for Cybersecurity (CIC) at the University of New Brunswick. It was created to provide a modern benchmark for training and evaluating intrusion detection systems (IDS) using machine learning and anomaly detection methods.

### Key Features

- **Realistic traffic patterns**: Includes both benign user activity and malicious attacks
- **Comprehensive attack coverage**: Contains major categories of cyberattacks including:
  - Brute Force attacks (FTP, SSH)
  - DoS/DDoS attacks
  - Web Attacks (XSS, SQL Injection)
  - Botnet activity
  - Port scanning and infiltration
- **Research relevance**: Widely recognized as one of the most comprehensive IDS datasets for academic research and cybersecurity system development

## Team Members ( Group 15 ) 

Taleb Jarrar      	    220911893   
Shahem hasunoglu  	    2409015433
Omar rasas		    220911745   
Rayyan Salameh	    220901690 
Ahmed A.S Abubreik     220901525 
Mohammad Rahmani     220901659   


## Repository Structure

This section will be updated as the project progresses. The repository will include:
- Dataset files
- Analysis notebooks/code
- Results and visualizations
- Documentation

Thanks I received the invitation. I do confirm I can access the documents. Group 15 // Please add this at the evry beginning in the project report name. Mennan Guder

PHASE 2 Readme file 

 MTH2526 – Data Mining for Cybersecurity  
 Project Phase 2 – Data Mining  
 Group 15

---

##  Project Overview
This project focuses on applying data mining and machine learning techniques for cybersecurity intrusion detection using the *CICIDS2017 dataset*.  
The goal is to preprocess large-scale network traffic data, perform exploratory data analysis (EDA), apply feature selection, and evaluate classification models for detecting different types of cyberattacks.

---

##  Dataset
- *Dataset Name:* CICIDS2017
- *Source:* Canadian Institute for Cybersecurity
- *Format:* CSV
- *Total Files:* 8
- *Original Rows:* 2,830,743
- *Columns:* 79
- *Labels:* Benign and multiple attack types (DDoS, DoS, PortScan, Web Attacks, Infiltration, etc.)

Each CSV file represents network traffic collected during different working days and attack scenarios.

---

##  Tools & Technologies
- *Programming Language:* Python 3
- *Libraries Used:*
  - pandas
  - numpy
  - scikit-learn
  - imbalanced-learn (SMOTE)
  - matplotlib
  - seaborn

---

##  Data Preprocessing
The preprocessing pipeline includes:
1. Loading and merging 8 CSV files into a single DataFrame
2. Duplicate detection and removal (10.89% of rows removed)
3. Handling missing and infinite values
4. Class imbalance handling using *SMOTE*
5. Feature scaling using *StandardScaler*
6. Feature selection using the *Chi-Square test* (Top 20 features selected)

---

##  Exploratory Data Analysis (EDA)
EDA was performed to understand data distribution and attack behavior:
- Class distribution analysis
- Correlation heatmap of selected features
- Histograms for key traffic features
- Boxplots comparing benign vs attack traffic
- Scatter plots and pair plots for class separability

Key insights include:
- Severe class imbalance in raw data
- Attack traffic generally shows longer flow durations and higher packet counts
- Some features are highly correlated, indicating redundancy

---

##  Data Mining Techniques
### Classification Models Applied:
1. *Random Forest Classifier*
   - High accuracy and robustness
   - Excellent performance on high-volume attacks

2. *Multi-Layer Perceptron (MLP)*
   - Used for comparison
   - Moderate performance compared to Random Forest

The dataset was split into *80% training* and *20% testing* using stratified sampling.

---

##  Results Summary
| Model | Accuracy | Precision | Recall | F1-score |
|------|---------|-----------|--------|----------|
| Random Forest | ~0.95 | ~0.95 | ~0.95 | ~0.95 |
| MLP | ~0.80 | ~0.85 | ~0.80 | ~0.79 |

Random Forest achieved the best overall performance and proved to be the most reliable model for intrusion detection.

---

##  Threat Detection Analysis
- High detection accuracy for common attacks such as *DDoS, **DoS, and **PortScan*
- Lower performance on rare attacks such as *Infiltration* and *Heartbleed*, even after applying SMOTE

---

##  Repository Structure
├── data/
│   └── sample_data.csv
├── notebooks/
│   └── preprocessing_eda_modeling.ipynb
├── figures/
│   └── plots_and_visualizations.png
├── README.md
└── requirements.txt
---
# MTH2526 – Data Mining for Cybersecurity  
## Project Phase 2 – Data Mining  
### Group 15

---

##  Project Overview
This project focuses on applying data mining and machine learning techniques for cybersecurity intrusion detection using the *CICIDS2017 dataset*.  
The goal is to preprocess large-scale network traffic data, perform exploratory data analysis (EDA), apply feature selection, and evaluate classification models for detecting different types of cyberattacks.

---

##  Dataset
- *Dataset Name:* CICIDS2017
- *Source:* Canadian Institute for Cybersecurity
- *Format:* CSV
- *Total Files:* 8
- *Original Rows:* 2,830,743
- *Columns:* 79
- *Labels:* Benign and multiple attack types (DDoS, DoS, PortScan, Web Attacks, Infiltration, etc.)

Each CSV file represents network traffic collected during different working days and attack scenarios.

---

##  Tools & Technologies
- *Programming Language:* Python 3
- *Libraries Used:*
  - pandas
  - numpy
  - scikit-learn
  - imbalanced-learn (SMOTE)
  - matplotlib
  - seaborn

---

##  Data Preprocessing
The preprocessing pipeline includes:
1. Loading and merging 8 CSV files into a single DataFrame
2. Duplicate detection and removal (10.89% of rows removed)
3. Handling missing and infinite values
4. Class imbalance handling using *SMOTE*
5. Feature scaling using *StandardScaler*
6. Feature selection using the *Chi-Square test* (Top 20 features selected)

---

##  Exploratory Data Analysis (EDA)
EDA was performed to understand data distribution and attack behavior:
- Class distribution analysis
- Correlation heatmap of selected features
- Histograms for key traffic features
- Boxplots comparing benign vs attack traffic
- Scatter plots and pair plots for class separability

Key insights include:
- Severe class imbalance in raw data
- Attack traffic generally shows longer flow durations and higher packet counts
- Some features are highly correlated, indicating redundancy

---

##  Data Mining Techniques
### Classification Models Applied:
1. *Random Forest Classifier*
   - High accuracy and robustness
   - Excellent performance on high-volume attacks

2. *Multi-Layer Perceptron (MLP)*
   - Used for comparison
   - Moderate performance compared to Random Forest

The dataset was split into *80% training* and *20% testing* using stratified sampling.

---

##  Results Summary
| Model | Accuracy | Precision | Recall | F1-score |
|------|---------|-----------|--------|----------|
| Random Forest | ~0.95 | ~0.95 | ~0.95 | ~0.95 |
| MLP | ~0.80 | ~0.85 | ~0.80 | ~0.79 |

Random Forest achieved the best overall performance and proved to be the most reliable model for intrusion detection.

---

##  Threat Detection Analysis
- High detection accuracy for common attacks such as *DDoS, **DoS, and **PortScan*
- Lower performance on rare attacks such as *Infiltration* and *Heartbleed*, even after applying SMOTE

---

##  Repository Structure
├── data/
│   └── sample_data.csv
├── notebooks/
│   └── preprocessing_eda_modeling.ipynb
├── figures/
│   └── plots_and_visualizations.png
├── README.md
└── requirements.txt
---
## ▶️ How to Run the Notebook
1. go to https://www.kaggle.com/code/mohammedrahmaniii/person2-datapreprocessing-final
2. Open the Kaggle Notebook 
3. Ensure the CICIDS2017 CSV files are available in the input directory  
4. Run the notebook cells sequentially from top to bottom  
5. The notebook will perform preprocessing, EDA, feature selection, and model training  
6. Results and visualizations will be displayed within the notebook
