# Trading-Preparation

## Creating a watchlist for the coming trading day 

*Please note that the source data was downloaded from barchart.com*

This entire process was centred around momentum. [Investing.com](investing.com) defines momentum investing as a trading strategy in which investors buy securities that are rising and sell them when they look to have peaked, where the goal is to work with volatility by finding opportunities in short-term uptrends and then sell when the securities start to lose momentum. This was my exact thinking in creating a process to select securities to include in the watchlist for trading. There are many momentum factors that are observable, however some are more reliable than others. I decided to foceus on these to preveent analysis paralysis and an information overload. These factors also proved to be consistent as leading indicators of stock price moves. I have listed them below:

### 🔴 Pre-market movers:
This section identifies stocks that had the biggest pre-market moves. There are several reasons why a stock would move in premarket hours, such as earnings anouncments, significant news of mergers, acquisitions or takeovers. These are events that significantly impact the price of a stock and their effects tend to spill over into the next trading session. Pre-market trading gives a retail investor with an opportunity to react to overnight news before the regular trading session starts. 

### 🟣 Most active:
This section shows the stocks that had the most volume during the presious trading session. Volume measures the number of shares traded in a stock or contracts traded in futures or options. Volume can indicate market strength, as rising markets on increasing volume are typically viewed as strong and healthy. When prices fall on increasing volume, the trend is gathering strength to the downside. When prices reach new highs (or no lows) on decreasing volume, a reversal might be taking shape. My application of volume in the process followed the logic that an increase in volume at the beginning of a trend indicated that the new trend is showing strength

### 🟢 Top performers
Top performers are stocks that moved the most during the previous trading session. Depending on the market structure these stocks are often ones that show signs of a strong trend. The goal is to catch these trends when they are still in the early stages to capture as much of the move as possible.

#### 🕸️ Cross referencing 
After extrating the 3 sections above from the raw data, its time to move on the most important step: putting them together. I made a decision to only combine a maximum of two features to prevent the filtering out of securities with potential to offer good returns that couldn't meet one of the criterias. Such as a top performer without a pre-market move. To that end, I came up with 3 different results:

- Pre-market movers 🔗 most active: stocks that moved premarket after showing high volume in the previous trading session
- Most active 🔗 top performers: stocks that showed the highest volume and made the biggest moves in the previous trading session
- Pre-market movers 🔗 top performers: stcoks that moved the most in the previous trading session and moved premarket 

##### Cross referencing the cross referenced securities
As an extra(optional) step, I also combined the different categories to come up with a much shorter list of high probability equities that appeared in more than one list. This watchlist was typically much shorter than the preceeding ones and in some rare cases it was empty!

[^note]as a last note, this entire session was done a few hours before the NY open to allow for research on stocks that made it to the final watchlist, for that I was looking for news that may explain the stocks behaviour. I used webull and yahoo finance for this
