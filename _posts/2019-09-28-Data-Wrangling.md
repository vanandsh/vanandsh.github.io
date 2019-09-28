## Data Wrangling

Crude oil itself has little or no value. But after undergoing various levels of processing like desalting, distillation, purification, extremely useful products like petroleum, gasoline and fuel-gases are obtained.
Drawing a similar parallel, real-world data by itself is usually dirty and doesn't adhere to any structure. Transforming such raw data into information that is of immense value and can be easily accessed is popularly known as Data Wrangling.

All algorithms and models require well-formatted structured data to perform optimally. Accordingly, this makes data wrangling one of the most critical and time-consuming processes in the entire pipeline of data science. In this blog, we will work through the popular Titanic challenge in Kaggle, using pandas(python library) to explain data wrangling.

[Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)

The objective of the challenge is to predict if a passenger would survive given their details. The challenge has three data sets - train.csv, test.csv and gender_submission.csv. 

<img src='./img/wrangling_steps.png' />

Data Wrangling process can be broken down into the steps below - 
1. Gather the correct data
2. Learn about the data 
3. Clean up your data
4. Organize your data
5. Create new data


**Gather the correct data**

The general idea is not to limit yourself to a particular system or data set. Tons of open-source data sets can be leveraged to get a better output. In our case, we already have the data sets provided. We'll use the train.csv for our example.

# Loading data into a dataframe using pandas

# Importing required libraries
import pandas as pd

# get titanic train csv files as a DataFrame
train_df = pd.read_csv('./titanic/train.csv')

print('Dimensions of train_df dataset: {0}'.format(train_df.shape))

