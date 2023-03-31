# Medical Insurance Cost Prediction
This repository contains a dataset and code for predicting medical insurance costs based on various factors such as age, gender, BMI, smoking status, and region.

## Dataset
The dataset is in CSV format and contains information on medical insurance costs for 1338 individuals. The following variables are included:

- Age: age of primary beneficiary
- Sex: gender of primary beneficiary (male or female)
- BMI: body mass index (kg/m^2) of primary beneficiary
- Children: number of children covered by insurance
- Smoker: smoking status of primary beneficiary (yes or no)
- Region: the beneficiary's residential area in the US (northeast, southeast, southwest, or northwest)
- Charges: individual medical insurance costs billed by the insurance company

## Data Understanding:
After loading the dataset using Pandas, we performed the following operations to better understand the data:

- Checked the shape of the dataset using df.shape
- Checked the data types of each column using df.info()
- Checked summary statistics of the numerical columns using df.describe()
- Checked for any missing values using df.isnull().sum()

## Exploratory Data Analysis:

We used various visualization techniques to explore the data and gain insights into the relationships between different variables. Here are some of the plots we generated:

- Count plot for the number of males and females
- Count plot for the number of smokers and non-smokers
- Count plot for the number of children in each family
- Count plot for the number of people in different regions
- Box plots for the distribution of BMI and insurance charges
- Box plot for the distribution of insurance charges with respect to sex
- Scatter plot for BMI vs insurance charges
- Scatter plot for age vs insurance charges
- Scatter plot for BMI vs insurance charges with respect to smoking and sex
The count plots showed that our dataset had slightly more males than females, and that the majority of people in the dataset were non-smokers. Most families had 0 or 1 child, and there were a similar number of people from each region.
The box plots showed that BMI and insurance charges had a positively skewed distribution, with a few outliers on the higher end. Additionally, the box plot for insurance charges with respect to sex showed that males had slightly higher charges on average than females.
The scatter plots showed a positive correlation between BMI and insurance charges, as well as between age and insurance charges. The scatter plot for BMI vs insurance charges with respect to smoking and sex showed that smokers tended to have higher charges than non-smokers, and that the relationship between BMI and charges was stronger for smokers than non-smokers. Additionally, the relationship between BMI and charges was stronger for females than males.

## Models
We use Linear Regression and Random Forest Regressor Models.
- With Linear Regression we get 0.78 r2-score.
- With Random Forest Regressor we get 0.86 r2-score.
