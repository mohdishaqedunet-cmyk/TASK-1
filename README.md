# TASK-1
The Titanic dataset is first loaded using Pandas to examine its structure by displaying the initial and final records. By inspecting names and values, features are manually classified into numerical, categorical and binary. The df.info() and df.describe() functions are used to analyse data types, identify missing values.

# titanic_data_loading.py
import pandas as pd

 # Load dataset
df = pd.read_csv("/content/train_and_test2.csv")

 # First 5 records
df.head()

 # Last 5 records
df.tail()
