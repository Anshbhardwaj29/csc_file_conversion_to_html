# csc_file_conversion_to_html
#pip install pandas
#pip install pandas-profiling------ you need to install these libraries for converting csv file raw data to html code
import pandas as pd
from pandas_profiling import ProfileReport

df = pd.read_csv('estadistical.csv')
# print(df)

# Generate a report
profile = ProfileReport(df)

profile.to_file(output_file="output1.html")
