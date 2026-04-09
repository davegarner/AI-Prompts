-----------------------------------------------------
Bitcoin Information - API Prompt
-----------------------------------------------------




-----------------------------
Prompt
-----------------------------





Please create a html based website that tracks bitcoin.  
The site will be hosted on Windows Server 2025 IIS 10
Please theme the site in the style of the TV series Severance
For content on the website please use enhanced markdown
Create a header and footer page so that links to the various pages can be updated easily
The site should be a pure client side api-fetch using the blockchain.com API

Please create a home page which links to  3 dashboards:

Bitcoin:
Current bitcoin price in USD - Auto-refresh this every 60 seconds
Current Market Cap
Current Hash Rate
Current Difficulty
Current Fees and colour coded to be low, medium and high
The current Block Height
Number of days until the next halving
Please ensure that the numbers fit in each section and perform rounding for extremely large numbers and should the actual number in smaller fonts for clarity

Price Chart:
A price chart that displays a line graph that displays different periods including:
1d, 1 week, 1 month, 3 months, 6 months, YTD, 1 Year, 5 Years, 10 years and All time
Include 50MA, 100MA 200MA and 300MA (moving Average across periods) toggles
Offer a selection of charts to display the data in different formats
Each chart should be zoomable to increase the resolution of the data

Currency Pairs:
Display different pairs in a tile format with the following pairs
BTC/USD
BTC/GBP
BTC/EUR
BTC/AUD
BTC/NZD
BTC/SGD
BTC/CAD
Colour code each of the pairs:
Red - Price gone down since the last refresh
Green - Price Gone up since the last refresh
Yellow - No price change since the last refresh

Please also create an about page.



please could you have a look at the dashboard 1, the numbers are too big due to the number of digits in the coin market cap

in dashboard 1, the difficulty is not displayed, if this is not presented by the coinbase api could you use the blockchain.com api instead to provide this info

in dashboard 2, there is a slight problem with the 200ma, it should be a toggle for each timeframe in the chart

can you make the graph in dashboard 2 zoomable?
also can you add another toggle which is 50MA where the MA is for the last 50 periods

