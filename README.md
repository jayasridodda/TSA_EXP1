# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 

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
Developed by: DODDA JAYASRI
REGISTER NO: 212222240028
```
```
import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv("Salesforcehistory.csv", nrows=100)
data["Date"]=pd.to_datetime(data["Date"])
plt.plot(data['Date'], data['Open'], label='Time Series Data')
plt.grid(True)
plt.title('Time Series Data Plot')
plt.xlabel('Date')
plt.ylabel('Open')
plt.legend()
plt.show()
```


# OUTPUT:

![Screenshot 2024-08-16 094737](https://github.com/user-attachments/assets/51e1e271-97b0-410d-bcc8-b31ac8430d56)





# RESULT:
Thus we have created the python code for plotting the time series of given data.
