# PySpark_Pipeline_Model_on_Databricks

## Introduction:



## Data:

The data used for this project is a set of credit card applications.  
https://archive.ics.uci.edu/ml/datasets/credit+approval

## Requirements:

```Pandas API on Spark:``` High-level API in Python for Apache Spark. It allows users to take advantage of the scalability and distributed computing capabilities of Spark while using the familiar and easy-to-use data structures and data analysis tools of Pandas.

```PySpark MLlib:``` A scalable machine learning library built on top of Spark. It consists of common learning algorithms and utilities. It is mainly used to take advantage of the parallel processing capabilities of Spark. 

## Description:

After reading the dataset located in the Databricks FileStore folder, the Pyspark dataframe is transformed into a pandas API on Spark dataframe. Preprocess steps like converting data types or imputing missing values are performed.

Once the dataframe is well prepared, a pipeline model is created comprising several stages like string indexers, vector assembler, or the random forest classifier.

Then, using the CrossValidator and the ParamGridBuilder tools, the pipeline model is trained in order to find the best hyperparameters to solve the problem.

Finally, the best model is selected and the best parameters are shown. A feature importance analysis is also displayed to measure the contribution of each variable to the model predictions.

