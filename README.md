GluonTS stock market S&P500 prediction deep learning light-weight Jupyter Notebook. The data used is from the early 1950s to March 24, 2020 which has two columns: timestamp, value 

<b>Time Stamp</b> contains the date and time 00:00:00 of the trading day
<b>Value</b> contains the CLOSE price for the trading day.

We will be predicting the CLOSE price for the trading days for 365 days from March 24, 2020 see the output below at 2000 epochs and a epoch loss rate of 1.98

<img src="https://i.ibb.co/0j8jgn6/Screen-Shot-2020-03-26-at-8-17-45-AM.png" alt="stock prediction s&p500 2020 365 days from now" border="0">

Dependencies:
1) Install GluonTS & MXNet https://gluon-ts.mxnet.io/install.html
2) Install Jupyter Notebook + Python==<3.6
3) Download dataset from Kaggle https://www.kaggle.com/codykrecicki/sp-500-1950-to-march-2020historicaldata

How to open notebook:
1) Use the command python3 -m notebook in your terminal
2) File -> Open -> sp500forcastmodel1.ipynb
3) Press the |> button thats says run, click it each time.

To change the time series prediction plot so you can see the predictions from a shorter previous time period than from 1950 like the examples below. Find <b>to_pandas(test_entry)[-30000:].plot(figsize=(20,13),linewidth=1)\n",</b> in the code and change <b>[-30000]</b> to another lesser negative number (play around with it to understand it). See examples below.
<img src="https://i.ibb.co/xjQm6cL/Screen-Shot-2020-03-26-at-8-17-11-AM.png" alt="stock prediction s&p500 2020 365 days from now" border="0">
<img src="https://i.ibb.co/7pPPKp1/Screen-Shot-2020-03-26-at-8-16-01-AM.png" alt="stock prediction s&p500 2020 365 days from nowM" border="0">

<i>Bugs to be fixed</i>:
x-axis is not showing the correct dates on the forcasted plot, doesn't effect outcome of time series prediction.

<i>Things to be added</i>:
Output forcast data into a table & csv file with future date time stamp and close price.
