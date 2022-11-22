# Trading_Bot_Python
Cryptocurrencies are known for being incredibly volatile, with prices fluctuating dramatically even in
the space of minutes. Investors also have the opportunity to take part in cryptocurrency trading around the
world and at any hour of the day. Combined, these factors limit the effectiveness of human cryptocurrency
trading in several ways.
First, investors in many cases cannot react quickly enough to changes in price to achieve the optimal
trades that are theoretically available to them. Slowdowns in exchanges and transaction times further exacerbate this problem. Second, investors can simply not dedicate as much time to the cryptocurrency markets
as necessary to always achieve the best trades. Doing so would require round-the-clock monitoring of cryptocurrency exchanges all over the globe.
Fortunately for many investors, there are solutions to these issues. One of the primary solutions is bots.
Crypto trading bots are automated software that helps you to buy and sell cryptocurrencies at the correct
time. The main goal of these software is to increase revenue and reduce losses and risks. These applications
enable you to manage all crypto exchange account in one place. Many such programs allow you to trade for
Ethereum, Litecoin, Bitcoin (BTC), and more with ease.

Introduction :
Crypto bots analyze data, predict risk and buy and sell assets as per their calculations. They watch
the market and trade when certain market conditions are met. Most crypto trading bots work by connecting
directly to a cryptocurrency exchange. After the bot successfully connects to an exchange, it starts watching the market and waiting for certain events or changes in prices. Once it detects an event, it will either
send you a signal to take action or make a decision based on the rules you’ve defined and take the required
action (buy/sell) itself. Some bots can even take into account historical data to make more accurate decisions.
1
1 Advantages of Bots in trading :
-Bots are used by traders to take advantage of the cryptocurrency markets that trade 24/7 all over the
world.
-The advantage bots have over investors is they can react quicker.
-Meanwhile, most investors also don’t have the time to dedicate to always get the best trade—something
that bots can do.
-One key type of bot is the arbitrage bot, which looks to take advantage of price discrepancies across
exchanges.
2 Binance :
Binance is a cryptocurrency exchange which is the largest exchange in the world in terms of daily trading
volume of cryptocurrencies.It was founded in 2017 and is registered in the Cayman Islands.
Binance was founded by Changpeng Zhao, a developer who had previously created high frequency trading
software. Binance was initially based in China, but later moved its headquarters out of China following the
Chinese government’s increasing regulation of cryptocurrency.
Part III
Project :
3 Install packages :
3.1 What Is Technical Analysis TA ?
Technical analysis is a trading discipline employed to evaluate investments and identify trading opportunities by analyzing statistical trends gathered from trading activity, such as price movement and volume.
2
3.2 What is Python-Binance ?
The Binance API is a method that allows you to connect to the Binance servers via Python or several
other programming languages. With it, you can automate your trading. More specifically, Binance has a
RESTful API that uses HTTP requests to send and receive data.
4 Libraries used :
Pandas, Numpy, ta, Seaborn, Matplotlib, ...
3
5 Dataset :
5.1 Download Data
Download and retrieve our dataset from the binance platform, this dataset is made up of a table of 12
columns: Time, open, close, high, low, volume .... since 01/01/2018 until the hour code execution.
5.2 Organize the Data for analysis:
Clean Dataset, Remove some columns :
4
Numiric columns Close, High, Low, Open :
Convert Time and define it as index :
5
6
6 Training data, Testing data :
we divide the data into two parts: Training data 80% and Testing data 20%.
7 Data visualization :
We analyze Close price of BTC over time from 01/01/2018 to 29/01/2022.
Let’s use matplotlib to visualise the series.
7
Since all values are positive, you can show this on both sides of the Y axis to emphasize the growth.
A correlation heatmap is a heatmap that shows a 2D correlation matrix between two discrete dimensions, using colored cells to represent data from usually a monochromatic scale. The values of the first
dimension appear as the rows of the table while of the second dimension as a column.
8
8 Trading bot strategy :
Many traders use moving averages to place their trades.
9
The issue with this, as for almost all indicators, is if you want to trade on a short time frame it is very likely
that you will miss the exact right time to execute the trade.
In our situation we will use Moving Average 200 and 600.
Visualize SMA200 and SMA600 graphics :
Define the trading bot strategy :
We start with 100000 USDT and 0 BTC.
10
Firstly, we iterate through our table line by line, secondly we test if the graph of SMA200 is
above of SMA600 graph and we have a balance usdt, then we buy BTC.
If the graph of SMA600 is above of SMA200 graph and we have a balance BTC, then we sell
BTC.
11
Using the strategy we win 715353.249818794 USDT, if we start with 100000 USDT
If we have bought BTC with 100000 usdt since 01/01/2018 how much we will earn if we
sell them with the current price of BTC.(280078.3649357935 USDT)
