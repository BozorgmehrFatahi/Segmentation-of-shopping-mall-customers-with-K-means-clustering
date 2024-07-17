# Segmentation-of-shopping-mall-customers-with-K-means-clustering
# Data Preprocessing and KMeans Clustering

This repository contains a Python script for preprocessing data and performing KMeans clustering using scikit-learn.

## Code Explanation

The code provided demonstrates how to:
- Load data from a CSV file
- Handle missing values
- Encode categorical variables
- Scale numerical features
- Perform KMeans clustering
- Calculate silhouette score

## Usage

To use this script:
1. Ensure you have Python installed along with required libraries (NumPy, Pandas, scikit-learn).
2. Place your data file (e.g., 'mall_customers.csv') in the '../data' directory.
3. Run the script to preprocess your data and perform KMeans clustering.

## Steps

1. **Loading Data**: The script reads a CSV file named 'mall_customers.csv' located in the '../data' directory and stores it in a Pandas DataFrame.
2. **Preprocessor Class**: A class named Preprocessor is defined, which contains methods for handling missing values, encoding categorical variables, and scaling numerical features.
3. **Data Preprocessing**: An instance of the Preprocessor class is created with the input DataFrame. The handle_missing_values(), encoder(), and scale() methods are called sequentially to preprocess the data. The transform() method combines all preprocessing steps and returns the preprocessed DataFrame.
4. **KMeans Clustering**: A KMeans model with 2 clusters and automatic initialization is created. The model is fitted to the preprocessed data, and cluster labels are retrieved.
5. **Silhouette Score Calculation**: The silhouette score of the clustered data is calculated using the preprocessed DataFrame and cluster labels. The score is then normalized to a range of [0, 1] by adding 1 and dividing by 2.

Feel free to modify the code according to your specific requirements or dataset.
