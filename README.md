# Stock-Quote-TSA-and-Regression
Create a visualization to show the following in 15-minute intervals for each stock in the included data -
    Average spread (Ask - Bid), 
    Average total bin volume as a percent of the full day’s volume 
    Volume-weighted average price (VWAP)



a.The response variable will be: 
*.Normalized mid price return from the time of trade to the midpoint price at 10 seconds after the time of a trade. 
        Formula: ( (Mid (t+10) – Mid (t)) / Mid(t) ) / (Ask (t) – Bid(t)) 


b.Predictors are:
*.Bid Offer Imbalance, calculated as
(Nbb_agg_size – Nbo_agg_size )/(Nbb_agg_size + Nbo_agg_size) 
*.Trade sign: 
    1 if the last trade price is above the average of bid and ask price
    -1 if the last trade price is below the average of bid and ask price
*.Trade Size imbalance over the last 10 seconds: Trade size imbalance for any period can be calculated as:
    Sum ( Trade Sign x Trade Size ) 


Calculating the 15-second volatility (standard deviation of mid price returns) for SHOO in each 30 minute interval. The volatility in annualized terms. 
