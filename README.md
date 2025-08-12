# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 12/08/2025

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import numpy as np 
import pandas as pd 
import matplotlib.pyplot as plt
df = pd.read_csv("C:\\Users\\admin\\time series\\Netflix_stock_data.csv") 
df.head()
df1 = df.copy()
df1['Date'] = pd.to_datetime(df1['Date'])
df1.set_index('Date', inplace=True)
plt.figure(figsize=(12, 6))
plt.plot(df1.index, df1['Volume'], label='Volume ', color='blue')
plt.title('Stock Volume Over Time')
plt.xlabel('Date')
plt.ylabel('Volume')
plt.grid(True)
plt.legend()
plt.show()

```








# OUTPUT:

<img width="1400" height="677" alt="image" src="https://github.com/user-attachments/assets/a094c785-7281-4955-a9dd-e98e44836cd0" />





# RESULT:
Thus we have created the python code for plotting the time series of given data.
