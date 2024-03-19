# Python-Project_Google_Playstore
Description
This Python script aims to preprocess and prepare a dataset for model building. The dataset consists of information about mobile applications including their ratings, reviews, installs, sizes, prices, and categories. The preprocessing steps include handling missing values, outliers, and converting data types. Additionally, redundant columns are dropped, categorical columns are encoded, and the dataset is split into train and test sets for further analysis.

Tasks Completed
Import Required Libraries and Read Dataset: Necessary libraries are imported and the dataset is read into the environment.

Data Exploration: Initial exploration of the dataset is performed, including examining the first few samples, shape, and info of the data to understand different features.

Summary Statistics: Summary statistics of the dataset are generated, identifying columns that need to be worked upon for model building.

Duplicate Records: Duplicate records, if any, are identified and dropped.

Invalid Categories: Invalid categories in the 'Category' column are identified and dropped.

Missing Values in 'Rating' Column: Missing values in the 'Rating' column are handled by dropping them. Additionally, a new column 'Rating_category' is created by converting ratings to high and low categories.

Distribution of 'Rating_category': The distribution of the newly created column 'Rating_category' is checked and commented upon.

Outliers in 'Reviews' Column: The 'Reviews' column is converted to a numeric data type and outliers are handled using a log transformation approach.

Treatment of 'Size' Column: Non-numeric data in the 'Size' column is treated and converted into a suitable data type. Entries where size='Varies with device' are dropped.

Treatment of 'Installs' Column: Unwanted characters in the 'Installs' column are treated, and the column is converted into a suitable data type.

Treatment of 'Price' Column: Unwanted characters in the 'Price' column are removed, and the column is converted into a suitable data type.

Redundant Columns Dropping: Columns deemed redundant for analysis are dropped, including 'App', 'Rating', 'Genres', 'Last Updated', 'Current Ver', and 'Android Ver'.

Encoding Categorical Columns: Categorical columns are encoded for further analysis.

Segregation of Target and Independent Features: The target variable ('Rating_category') and independent features are segregated for model building.

Splitting the Dataset: The dataset is split into train and test sets.

Standardization: Data is standardized to ensure values are within a particular range.
