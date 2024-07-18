# Simple-imputation-technique-in-Python

Understanding the nature of missing data is crucial for choosing the appropriate method to handle it. Missing data can generally be categorized into three types:

##### Missing Completely at Random (MCAR)
##### Missing at Random (MAR)
##### Missing Not at Random (MNAR)

Types of Missing Data:


#### 1. Missing Completely at Random (MCAR)
Data is missing completely at random when the probability of a data point being missing is unrelated to any other data or any other variable in the dataset. In this case, the missing data is a random subset of the data, and there is no systematic pattern causing the data to be missing.

Example: A sensor fails intermittently due to random hardware issues, and thus some readings are missing randomly.

#### 2. Missing at Random (MAR)
Data is missing at random when the probability of a data point being missing is related to some other observed data but not the value of the missing data itself. In this case, the missing data may depend on other variables in the dataset but not on the variable with missing data.

Example: Suppose older patients are less likely to fill out certain sections of a medical questionnaire. The missingness is related to age (an observed variable) but not necessarily to the answers themselves.
#### 3. Missing Not at Random (MNAR)
Data is missing not at random when the probability of a data point being missing is related to the value of the missing data itself. This type of missing data introduces bias because the missingness is systematically related to the value that is missing.

Example: People with higher incomes may be less likely to report their income on a survey. The missingness is directly related to the income level itself.

### Handling Missing Data
The strategy for handling missing data depends on the type of missingness. Below are some common imputation techniques, which can be visualized using the iris dataset with introduced missing values.

#### Imputation Techniques

#### Mean Imputation:

Replace missing values with the mean of the column.

#### Median Imputation: 

Replace missing values with the median of the column.

#### Mode Imputation: 

Replace missing values with the mode of the column.



#### Forward Fill:

Replace missing values with the previous value in the column.



#### Backward Fill:

Replace missing values with the next value in the column.



#### K-Nearest Neighbors (KNN) Imputation:

K-Nearest Neighbors (KNN) Imputation fills missing values by finding the k-nearest neighbors of the missing data point and averaging their values. This method leverages the similarity between data points to provide more accurate imputations.


There are some ML techniques for imputation e.g., 

#### Multiple Imputation by Chained Equations (MICE)

#### Random Forest Imputation

#### Bayesian Imputation

#### Autoencoder Imputation

#### Matrix Factorization Imputation

#### Gradient Boosting Imputation
