# Customer Segmentation Project README

## Project Overview

This project aims to identify segments of the population that form the core customer base for a mail-order sales company in Germany. The goal is to use unsupervised learning techniques to cluster the general population into groups with similar demographic properties and then analyze how the customer data fits into these clusters. The data used in this project has been provided by our partners at Bertelsmann Arvato Analytics.

## Files Included

- `Identify_Customer_Segments.ipynb`: Jupyter Notebook containing the analysis steps.
- `Udacity_AZDIAS_Subset.csv`: Demographics data for the general population of Germany.
- `Udacity_CUSTOMERS_Subset.csv`: Demographics data for customers of a mail-order company.
- `Data_Dictionary.md`: Detailed information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv`: Summary of feature attributes for demographics data.

## Steps in the Project

### Step 0: Load the Data
- Load demographics data for the general population into a pandas DataFrame.
- Explore the structure of the dataset and the feature summary file.

### Step 1: Preprocessing
#### Step 1.1: Assess Missing Data
- Convert missing value codes to NaN.
#### Step 1.2: Select and Re-Encode Features
- Re-encode categorical features.
- Engineer mixed-type features.

### Step 2: Feature Transformation
#### Step 2.1: Apply Feature Scaling
- Scale the features to mean 0 and standard deviation 1.
#### Step 2.2: Perform Dimensionality Reduction
- Apply Principal Component Analysis (PCA).
#### Step 2.3: Interpret Principal Components
- Investigate and interpret feature associations from the first three principal components.

### Step 3: Clustering
#### Step 3.1: Apply Clustering to General Population
- Use k-means clustering to identify clusters in the PCA-transformed data.
#### Step 3.2: Apply All Steps to the Customer Data
- Preprocess, scale, apply PCA, and cluster the customer data using the general population models.
#### Step 3.3: Compare Customer Data to Demographics Data
- Compare the cluster distributions between general population and customer data.

## Discussion and Findings
- Report findings, decisions, and interpretations in the provided discussion cells.

## Conclusion
- Summarize key results and insights gained from the analysis.

## Dependencies
- Python 3
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## How to Run the Code
1. Install the required dependencies using `pip install -r requirements.txt`.
2. Open the Jupyter Notebook `Identify_Customer_Segments.ipynb` and run the cells in sequence.

Feel free to reach out for any questions or clarifications!

## Acknowledgments
This project is part of the Udacity Nanodegree program.