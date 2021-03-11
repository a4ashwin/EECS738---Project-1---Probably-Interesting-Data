# EECS738---Project-1---Probably-Interesting-Data

 Prerequisites
 Python 3.7.3, Jupyter Notebook, Pandas Library, Numpy Library & sklearn Library

 Introduction:
 In this project, we are going to build a heuristic and/or algorithm to model the data using mixture models of probability distributions programmatically.
 
 Datasets used:
 1. Haberman's Survival
	The dataset contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago's Billings Hospital on the survival of patients who had undergone 	surgery for breast cancer.
	Attribute Information:

	1. Age of patient at time of operation (numerical)
	2. Patient's year of operation (year - 1900, numerical)
	3. Number of positive axillary nodes detected (numerical)
	4. Survival status (class attribute)
	-- 1 = the patient survived 5 years or longer
	-- 2 = the patient died within 5 year

 2. Real estate valuation data set 
	The market historical data set of real estate valuation are collected from Sindian Dist., New Taipei City, Taiwan. The â€œreal estate valuationâ€ is a regression problem. The data 	set was randomly split into the training data set (2/3 samples) and the testing data set (1/3 samples).
	The inputs are as follows
	X1=the transaction date (for example, 2013.250=2013 March, 2013.500=2013 June, etc.)
	X2=the house age (unit: year)
	X3=the distance to the nearest MRT station (unit: meter)
	X4=the number of convenience stores in the living circle on foot (integer)
	X5=the geographic coordinate, latitude. (unit: degree)
	X6=the geographic coordinate, longitude. (unit: degree)

 Idea:
 We are going to implement the Expectation maximization algorithm which provides an iterative solution to maximum likelihood estimation with latent variables.
 There are two functions needed for that:
 Expectation : Estimation of probability of each Gaussian for the point they generate
 Maximization: Modify parameters according to the variables to maximize the likelihood of the data.

 Process:
 - Download the data from https://archive.ics.uci.edu/ml/datasets.php
 - Load the dataset into Pandas dataframe.
 - Drop the columns that are not significant in predicting the demand of the products.
 - Drop the rows with Nan(missing values) as they won't help in achieving our goal and also, they will create discrepancies in prediction.
 - Implement the EM Algorithm on the two downloaded datasets
 - Cluster the data in to multiple groups.

 Result:
 We have successfully implemented the Expectation maximization algorithm to cluster the data. We have successfully clustered the dataset with different number of attributes in to two clusters.

 Built With:
 Jupyter Notebook
 Python 3.7.3
 Pandas
 NumPy

 Authors:
 Ashwin Rathore

 License:
 This project is created for Course EECS 738 Assignment for University of Kansas.

 Acknowledgments:
 https://archive.ics.uci.edu/ml/datasets.php
 https://www.kaggle.com/charel/learn-by-example-expectation-maximization
 https://medium.com/analytics-vidhya/expectation-maximization-algorithm-step-by-step-30157192de9f
 https://machinelearningmastery.com/expectation-maximization-em-algorithm/
