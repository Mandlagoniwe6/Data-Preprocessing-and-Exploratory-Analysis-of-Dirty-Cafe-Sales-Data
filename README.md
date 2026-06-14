# Cafe Sales Data Preprocessing
## Overview
This project cleans and prepares a dirty cafe sales dataset for machine learning.

## Dataset Issues Addressed
- Missing values (up to 39.6% in some columns)
- Placeholder errors ("ERROR", "UNKNOWN")
- Mixed data types
- Inconsistent date formats

## Preprocessing Steps
### 1. Data Cleaning
- Converted numerical columns to proper types
- Replaced placeholders with NaN
- Dropped unrecoverable rows

### 2. Missing Value Handling

Column	          Missing %	    Method Used
Location	        39.6%	        Dropped column
Payment Method	  31.8%	        Created 'Missing' category
Quantity	        8.2%	        Median imputation
Price Per Unit	  8.8%	        Median imputation
Transaction Date	4.6%	        Dropped rows
### 3. Feature Engineering
- Extracted Day_of_Week, Month, Is_Weekend from Transaction Date

### 4. Encoding
- One-hot encoding for Payment Method
- Frequency encoding for Item

## Visualisations Created
- Histograms of numerical variables
- Boxplots for outlier detection
- Correlation heatmap
- Missing data matrix
- Missing percentage bar chart

## Results
- Original rows: 10,000
- Final rows: 9,942
- Final features: 15+

## Files
- `data_preprocessing.ipynb` - Complete preprocessing code
- `report.pdf` - Detailed project report

## Requirements
- Python 3.x
- pandas, numpy, matplotlib, seaborn, missingno, scikit-learn
