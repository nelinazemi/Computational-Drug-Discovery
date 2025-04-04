# Computational Drug Discovery for **Acetylcholinesterase Inhibitors**  

This project focuses on analyzing potential drug candidates for **Acetylcholinesterase (AChE) inhibition**, which is relevant in treating neurodegenerative diseases like **Alzheimer's disease**. The pipeline involves data extraction, preprocessing, feature engineering, and machine learning for predictive modeling.  

## Features:
- **Data Collection**: Extracts bioactivity data from the **ChEMBL** database, focusing on compounds targeting Acetylcholinesterase (AChE).  
- **Preprocessing**: Cleans missing values, classifies compounds into **active, inactive, and intermediate** based on IC50 values, and computes molecular descriptors.  
- **Molecular Descriptor Calculation**: Uses **RDKit** to extract chemical properties such as Molecular Weight, LogP, Hydrogen Bond Donors, and Acceptors.  
- **Exploratory Data Analysis (EDA)**: Visualizes the distribution of molecular properties and their correlation with bioactivity.  
- **Machine Learning Model**: Implements **RandomForestRegressor** and **LazyPredict** to predict drug potency using quantitative structure-activity relationship (QSAR) modeling.  
- **Feature Selection**: Uses **variance thresholding** to remove redundant descriptors.  

## Requirements:
- Python 3  
- Google Colab  
- ChEMBL API  
- RDKit  
- Seaborn & Matplotlib  
- LazyPredict  

## Dataset:
- **ChEMBL Bioactivity Data** (Acetylcholinesterase inhibitors)  
- **Kaggle Dataset** for extended model training  

## Installation:
Run the following in Google Colab:  
```python
!pip install chembl_webresource_client rdkit lazypredict
```

## Usage:
1. Mount Google Drive and copy the dataset  
2. Preprocess and clean the data  
3. Extract molecular descriptors using RDKit  
4. Train machine learning models to predict **AChE inhibition potency**  
