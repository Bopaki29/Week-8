# Week-8
🦠 COVID-19 Tracker for South Africa's Provinces
 Data Analysis Project Using Python

What This Project Does 
We are building a simple project to understand how COVID-19 spread in different provinces of South Africa. We’ll use a real dataset, clean it up, look at the numbers, and draw graphs to help understand:
-Total cases

-Total deaths

-Vaccinations

-Daily changes
#  Step 1: Get the Data
import pandas as pd


url = "https://raw.githubusercontent.com/dsfsi/covid19za/master/data/covid19za_provincial_cumulative_timeline_confirmed.csv"

df = pd.read_csv(url)

print(df.head())

# out come 










import pandas as pd

# GitHub raw CSV URL from the DSFSI COVID-19 repo
url = "https://raw.githubusercontent.com/dsfsi/covid19za/master/data/covid19za_provincial_cumulative_timeline_confirmed.csv"

# Load the CSV file directly from the URL
df = pd.read_csv(url)

# See what the data looks like
print(df.head())

         date  YYYYMMDD   EC   FS   GP  KZN   LP   MP   NC   NW   WC  UNKNOWN  \
0  05-03-2020  20200305  0.0  0.0  0.0  1.0  0.0  0.0  0.0  0.0  0.0      0.0   
1  07-03-2020  20200307  0.0  0.0  1.0  1.0  0.0  0.0  0.0  0.0  0.0      0.0   
2  08-03-2020  20200308  0.0  0.0  1.0  2.0  0.0  0.0  0.0  0.0  0.0      0.0   
3  09-03-2020  20200309  0.0  0.0  1.0  6.0  0.0  0.0  0.0  0.0  0.0      0.0   
4  11-03-2020  20200311  0.0  0.0  5.0  7.0  0.0  0.0  0.0  0.0  1.0      0.0   

   total source  
0      1    NaN  
1      2    NaN  
2      3    NaN  
3      7    NaN  
4     13    NaN  
