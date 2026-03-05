# Comprehensive-Titanic-EDA-with-Visualizations-and-Key-Findings
This commit updates the repository with the final, detailed Exploratory Data Analysis (EDA) of the Titanic dataset. The work is contained in the original_titanic_eda.ipynb notebook and uses the train_dataset(1).csv.
Key Activities and Analysis Steps:

Data Loading and Initial Inspection:

Loaded the dataset train_dataset(1).csv.

Inspected the data structure using .info(), .describe(), and .shape.

Identified missing values across features, particularly in 'Age', 'Cabin', and 'Embarked'.

Data Cleaning:

Handled missing values in the 'Age' column by filling with the median (to avoid influence of outliers).

Addressed missing 'Embarked' values by filling with the mode.

Dropped the 'Cabin' column due to an excessive amount of missing data (approx. 77%).

Verified the removal of all null values.

Exploratory Data Analysis (EDA) & Visualization:

Conducted a univariate and bivariate analysis using statistical functions and visualizations.

Utilized key Python functions for analysis:

seaborn.countplot(): To visualize frequency distributions of categorical variables.

seaborn.histplot(): To examine the distribution and frequency of numerical variables like 'Age' and 'Fare'.

seaborn.heatmap(): To analyze correlation between features and identify relationships.

matplotlib.pyplot.figure() and related functions to create and manage the visualizations.

Key Findings (Transcribed from Handwritten Notes):

Gender: Females had a significantly higher survival rate (approx. 74%) compared to males (approx. 19%).

Passenger Class: Class 1 passengers had the highest survival rate, while Class 3 had the lowest.

Age: Children had a better chance of survival than other age groups.

Age Distribution: The majority of passengers were in the age range of 20 to 30 years.
