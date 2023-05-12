# EDA_and_Model_Building
We will explore blueberry yield dataset from kaggle and perform Exploratory Data Analysis and Build few machine learning models to predict the yield

The analysis starts with installing and importing the necessary libraries for data analysis, such as Optuna, NumPy, Pandas, Seaborn, LightGBM, and others. The dataset used in the analysis consists of two files: "train.csv" and "test.csv," which are read into separate DataFrames along with an additional "original" DataFrame containing the original dataset.

After loading the data, the columns "id" and "Row#" are dropped from the train and original DataFrames, respectively, as they are not relevant for the analysis.

New features are then created based on the existing columns in the train DataFrame. These features include "total_bee_density," "temp_range," "temp_deviation," "pollination_potential," "yield_potential," and "total_seeds." These features aim to capture additional information and patterns from the existing data.

Next, exploratory data analysis (EDA) and statistical analysis are performed on both the target column ("yield") and the feature columns. The EDA includes visualizations of the distribution, skewness, and outliers in the data. Statistical analysis involves calculating summary statistics, detecting outliers using z-scores, and examining the skewness of the data through Q-Q plots.

Key observations from the analysis include:

The target column ("yield") is normally distributed with a slightly negative skewness.
There are no missing values in the dataset.
Multimodal distributions are observed in some of the feature columns.
Outliers are detected in the honeybee column and require further investigation.
Some columns exhibit high correlation with the target column, indicating their potential importance in predicting the target variable.
No duplicate rows are found in the dataset.
Finally, the analysis concludes with feature scaling using StandardScaler. However, the code provided in the question is incomplete, as the fitting and transformation steps are missing.

In summary, the analysis provides an overview of the dataset, explores the distribution and relationships between variables, detects outliers, and prepares the data for further analysis or modeling.
