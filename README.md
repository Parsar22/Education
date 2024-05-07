# Exploring the Relationship Between Socioeconomic Factors and School Performance on Standardized Tests

## description
This project aims to investigate whether socioeconomic factors influence school performance on standardized tests, specifically the ACT or SAT exams in U.S. high schools.
## Data 
This project utilizes two data sets [EdGap_data.xlsx](https://github.com/Parsar22/Education/blob/1ef80dbb86f98226108ed3cc586b3e162da545f7/EdGap_data.xlsx) and [ccd_sch_029_1617_w_1a_11212017.csv](https://drive.google.com/file/d/1HvW2w-o2XZzCm4KTvnb1Bb3BvoAa14BP/view?usp=sharing). The primary data set is the EdGap data set from [EdGap.org](https://www.edgap.org/#5/37.875/-96.987). This data set from 2016 includes information about average ACT or SAT scores for schools and several socioeconomic characteristics of the school district. The secondary data set is basic information about each school from [the National Center for Education Statistics](https://nces.ed.gov/ccd/pubschuniv.asp).

## Requirements

Software:
Python 3+
pandas (for data manipulation)
NumPy (for numerical computations)
Seaborn or Matplotlib (for visualizations)
scikit-learn (for machine learning models)

## Data Preperation

Steps Undertaken:
Initial Data Inspection: conducted an exploratory analysis to understand the datasets' structure and content.

Data Cleaning: This included converting data types, handling out-of-range values, and removing unnecessary parts like duplicates.

Merging Datasets: The EdGap dataset was merged with the school information dataset using school IDs to create a unified analysis base.

Identifying Missing Values: We identified missing values across the merged dataset to strategize their imputation.

Train-Test Split: The data was split into training and test sets to facilitate a clean imputation process and avoid data leakage.

the colab notebook used for data preperation can be accessed [here](https://github.com/Parsar22/Education/blob/main/DATA_3320_Education_Inequality_Data_Preparation.ipynb) and cleaned data [testing_data.csv](https://github.com/Parsar22/Education/raw/main/testing_data.csv) and [training_data.csv](https://github.com/Parsar22/Education/raw/main/training_data.csv) can be accessed from these links

Data Imputation: Using the IterativeImputer, we imputed missing values separately in the training and test datasets.

Feature Scaling: Post-imputation, we scaled the features to provide each with equal weight in the predictive modeling.

Exporting Cleaned Data: The final cleaned and processed data were exported as CSV files for further use.|


## Analysis

Data Exploration:

Calculated summary statistics to understand data characteristics.
Examined correlations between socioeconomic factors and ACT scores to identify key relationships.
Visualized the relationship between free lunch percentage and ACT scores using a scatterplot.
Created a bar chart to compare ACT scores across different income levels within states.
Predictive Modeling:

Built a linear regression model and Random Forest Model to predict ACT scores based on socioeconomic factors.
Developed a Random Forest model for potentially improved accuracy.
Evaluated both models using metrics like Mean Squared Error (MSE) and R-squared.


## Author 

Parsa Rahimiderimi

## License 

This project is open source and can be used with references


