# 🧬 End-to-End Oncology Survival Prediction & Clinical Risk Stratification
### *From Raw Electronic Health Records (EHR) to Stratified Cox Regression Models*

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Domain](https://img.shields.io/badge/Domain-Oncology%20%7C%20Biostatistics-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

## 🏥 Project Overview
In the realm of precision medicine, understanding patient prognosis is crucial for treatment planning. However, real-world clinical data extracted from **Hospital Information Systems (HIS)** is rarely "analysis-ready." It is often unstructured, inconsistent, and plagued by missing values.

This project simulates a comprehensive **Clinical Data Science workflow** using a high-fidelity synthetic dataset of **1,500 cancer patients**. The goal is not merely to fit a model, but to demonstrate the rigorous process of transforming "dirty" raw data into actionable medical insights.

**Key Objectives:**
1.  **Data Wrangling:** Cleaning "messy" clinical entries (e.g., *'Stage IV'* vs *'Metastatic'*, *'Lung CA'* vs *'nsclc'*).
2.  **Smart Imputation:** Handling missing biomarkers using **Domain-Driven Logic** (e.g., imputing *Tumor Size* based on *Clinical Stage* medians).
3.  **Survival Modeling:** Quantifying mortality risk using **Stratified Cox Regression** to satisfy Proportional Hazards assumptions.
4.  **Bias Detection:** Identifying and visualizing "Confounding by Indication" in chemotherapy outcomes.

---

## 📂 Project Structure
The repository is organized to simulate a production-level data science environment:

```text
├── data/
│   └── complex_oncology_data.csv   # The raw, synthetic "dirty" dataset
├── images/                         # Generated plots and visualizations
│   ├── cox_hazard_ratios.png
│   ├── kaplan_meier_plot.png
│   └── ...
├── survival_data_analysis.ipynb    # Main analysis notebook (The Code)
└── README.md                       # Project documentation
