# TASK-1
The Titanic dataset is first loaded using Pandas to examine its structure by displaying the initial and final records. By inspecting names and values, features are manually classified into numerical, categorical and binary. The df.info() and df.describe() functions are used to analyse data types, identify missing values.

# titanic_data_loading.py
import pandas as pd

df = pd.read_csv("/content/train_and_test2.csv")

df.head()

df.tail()

#titanic_data_overview.py
df.info()

df.describe()

#titanic_categorical_analysis.py
categorical_cols = df.select_dtypes(include=['object']).columns

for col in categorical_cols:

    print(f"\n{col}")
    
    print(df[col].value_counts())

    #titanic_data_cleaning_check.py
    df.isnull().sum()
