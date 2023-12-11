All data files are located in the "data" directory, each csv file contains data from one year from 1995 to 2023.

Preprocessing.ipynb is used to preprocess the raw data. During preprocessing, it:
	concatenates all data files into one pyspark dataframe,
	performs EDA on the dataset,
	fills in missing value,
	encodes all the categorical features,
	creates a data_preprocessed.parquet file to save the data after preprocessing.

Model.ipynb is used to make predictions. It:
	split the dataset into training and testing data,
	implements normalization and PCA, creates data_train_pca.parquet and data_test_pca.parquet files,
	builds 4 different models and trains them using cross validation and grid search.


