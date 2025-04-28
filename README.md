# Capstone Project - Predicting FDA Approval for Biological Products

## Overview
In this project, the primary objective is to perform **Exploratory Data Analysis (EDA)** and develop an initial report for the capstone project.  
EDA is used here to uncover insights beyond traditional modeling, hypothesis testing, and training tasks, helping to better understand variable relationships and data characteristics.

The project involves cleaning the data, performing feature engineering, and using EDA techniques to create meaningful visualizations. Additionally, a **baseline machine learning model** is developed as a comparison point for future model improvements.

## Research Question
**How can we predict whether a biological product will be FDA-approved or rejected based on its applicant, product type, dosage, and other features?**

## Data Source
- **FDA Purple Book**: Contains detailed information on FDA-licensed biological products, including biosimilars, interchangeable products, and reference products.
- Data accessed from the official FDA website: [FDA Purple Book Database](https://purplebooksearch.fda.gov/).

## Methodology

### Data Cleaning
- Converted categorical columns to `category` dtype for memory optimization and improved processing.
- Converted numerical columns using `pd.to_numeric`, coercing invalid entries.
- Handled outliers by clipping certain features to reasonable predefined ranges.
- Removed duplicate records to ensure data integrity.

### Exploratory Data Analysis (EDA)
- **Histograms** to observe distributions of numerical features.
- **Boxplots** to identify spread and potential outliers.
- **Correlation heatmaps** to detect relationships among numerical variables.
- Summary statistics for both categorical and numerical features.

### Feature Engineering
- Created a new binary target column `Approval_Status_binary` based on the approval status of the biological products.

## Machine Learning Models

For initial baseline modeling, the following **binary classification algorithm** were used:
- Logistic Regression


### Evaluation Metrics
The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score

## Expected Results
- Development of a classification model capable of predicting the FDA approval status of biological products.
- Identification of key product features (such as applicant, BLA type, dosage form, route of administration, and strength) strongly influencing the approval outcome.
- Insights into factors that are predictive of approval success or rejection.

## Importance of This Research Question
The FDA approval process for biological products is complex, costly, and uncertain.  
Predicting approval likelihood can assist:
- Manufacturers in strategic product development and resource allocation.
- Researchers in identifying critical success attributes.
- Stakeholders in planning market entry and managing regulatory risks.

Ultimately, a predictive model could help reduce uncertainties in the FDA process and accelerate patient access to innovative therapies.

## Deliverables
- Jupyter Notebook(s) containing:
  - Data cleaning steps
  - Feature engineering processes
  - EDA visualizations
  - Baseline machine learning models

