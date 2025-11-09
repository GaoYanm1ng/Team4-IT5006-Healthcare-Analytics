# IT5006 - Milestone 3 - Predicting Length of Stay and Discharge Destination in Hospitals

## Project Overview

Our project aims to enhance hospital operation efficiency and patient flow management by developing predive models for two critical outcomes: Length of Stay (LOS) and Discharge Destination. Utilising data in the Diabetes 130-US Hospital dataset, our goal is to provide hospitals with the capabilities to better manage bed shortages, optimize resource allocation and proactively arrange necessary post-discharge logistics. This multi-model approach help us address key areas in the patient journey that impacts hospital capacity.

## Dataset Information:
*    **Source**: UCI Machine Learning Repository - Diabetes 130-US Hospitals dataset
*    **Access**: https://github.com/uci-ml-repo/ucimlrepo
*    **Domain**: Healthcare/Hospital Management
*    **Size**: 101,766 patient encounters across 130 hospitals
*    **Time Period**: 1999-2008
*    **Features**: 50+ attributes covering demographics, clinical data, medications, and outcomes

## Project Objectives

1.  **Regression Task: Predicting Length of Stay**
    **Goal**: Our project is to build a predictive model for predicting patients’ length of stay in hospital (time_in_hospital) in the Diabetes 130-US Hospitals dataset, based on demographic, clinical and admission-related information.

2.  **Multi-Class Classification Task: Predicting Discharge Destination**
    **Goal**: Our project includes building a predictive model to anticipate a patient’s discharge destination utilizing the Diabetes 130-US Hospitals dataset. 

## Methodology

   For the data preprocessing, we focused on transforming the original complex dataset into a clean dataset which is more suitable for machine learning. According to the description on the dataset website, this dataset contains over 100,000 medical records and more than 50 features, which shows a real patient environment faced by diabetes hospitals. Therefore, the dataset has a large number of missing values, complex categorical features, and disordered categorical variables. To ensure the accuracy, completeness, and consistency of the data quality, we established data preprocessing work on the original dataset including data cleaning, classification filtering, feature engineering, and feature encoding.

3.  **Model Implementation & Evaluation**:
    In the regression problem section, we decided to take "length of hospital stay" as the core feature for prediction. We first adopted Train-Test Split as the framework for this feature evaluation. To be specific, we split the dataset into a ratio of 80% for training and 20% for testing in order to prevent overfitting of the model. Meanwhile, we set up fixed random seeds to ensure the reproducibility of all experimental results. All models are built on the dataset with detailed steps of data preprocessing discussed in the first part. Our modeling strategy will start with a simple linear model and gradually take in more complex ensemble learning models. Therefore, the analysis below will showcase the following algorithms:
    1. Linear regressor
    2. Random Forest Regressor
    3. Hist-Gradient Boosting Regressor.

    The goal of this problem is to predict the discharged_disposition_grouped target variable, which was created by grouping the original discharge_disposition categories into three main classes: 'Discharged Home', 'Transferred to Another Hospital', and 'Transferred to Facility-Based Care'. Our modeling strategy will start with a simple basic model and gradually take in more complex ensemble learning models. All models are built on the dataset with detailed steps of data preprocessing discussed in the first part. Therefore, the analysis below will showcase the following algorithms:
    1. Logistic Regression
    2. Decision Tree Classifier
    3. Random Forest Classifier
    4. XGBoost Classifier


## Setup and Installation

This project uses a Conda environment to manage dependencies. To set up the environment, please follow these steps:

1.  **Install Anaconda**: If you don't have it, download and install the Anaconda Distribution (64-bit) for your operating system (macOS or Windows).

2.  **Install Required Libraries**: 
    ```bash
    pip install pandas numpy scikit-learn xgboost matplotlib seaborn ucimlrepo jupyter
    ```

## How to Run

1.  **Activate the Environment**: Open your terminal and activate the Conda environment

2.  **Open and Run the Notebook**:  Navigate to the project directory, open the `Team4_Milestone2_IT5006_AY2526.ipynb` file, and run the cells sequentially from top to bottom to reproduce the entire analysis.

## Repository Structure

* `Team4_Milestone_2.ipynb`: The main Jupyter Notebook containing all data preprocessing, model training, and evaluation code.
* `Team4_Milestone2_IT5006_AY2526.pdf`: The final written report summarizing the project's methodology, results, and insights.
* `README.md`: This file, providing an overview and setup instructions for the project.
