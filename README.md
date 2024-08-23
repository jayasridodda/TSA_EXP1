### Developed By: DODDA JAYASRI
### Register No: 212222240028
###  Date: 
# Ex.No: 01A PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data (Sales Force history)
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Using pd.to_datetime we're coverting date/month/year to only year.
4. Plot the data according to need and can be altered yearly.
5. Display the graph.
# PROGRAM:

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
