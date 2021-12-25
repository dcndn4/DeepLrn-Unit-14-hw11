# DeepLrn-Unit-14-hw11
Deep Learning applied to Bitcoin 



![Deep Learning](Images/deep-learning.jpg)

Enclosed please find two Jupyter Lab notebooks, each modeling bitcoin closing prices using Recurrent Neural Networks (RNN's).  This modeling was done in two different ways: one model applies FNG indicators, while the other model is restricted to closing price data alone. 

FNG (Fear and Greed) indictors relate to the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/), which was launched by Alternative in January of 2018 ranges from 0 (“Extreme Fear”) to 100 (“Extreme Greed”); and is currently in the 'Fear' zone.

[FNG Index Dial](![image](https://user-images.githubusercontent.com/90283165/147389087-aa8dd046-8aa0-4305-b830-5848fc2b517f.png)

The Crypto Fear and Greed Index is based on three factors:

[] Price changes in major cryptocurrencies (bitcoin, ethereum, and ripple). The larger the change in price, the more important that this data becomes;

[] Volume for each of these cryptocurrencies. The greater the volume, the more important that this data becomes;

[] Volatility. This means how much a cryptocurrency fluctuates in price over time.

The fear and greed index was derived from the stock market-based fear and greed index developed by CNNMoney in 2014 related to investors purchases of pubicly-traded stocks. That original index was based on seven factors:


[] Stock Price Momentum - A measure of the Standard & Poor's 500 Index (S&P 500) versus its 125-day moving average (MA).

[] Stock Price Strength - The number of stocks hitting 52-week highs versus those hitting 52-week lows on the New York Stock Exchange (NYSE).

[] Stock Price Breadth - Analyzing the trading volumes in rising stocks against declining stocks.

[] Put and Call Options - The extent to which put options lag behind call options, signifying greed, or surpass them, indicating fear.

[] Junk Bond Demand - Gauging appetite for higher risk strategies by measuring the spread between yields on investment-grade bonds and junk bonds.

[] Market Volatility - CNN measures the Chicago Board Options Exchange Volatility Index (VIX) concentrating on a 50-day MA.

[] Safe Haven Demand - The difference in returns for stocks versus treasuries.

Behavioral economists find a strong correlation between emotion and behavior, and also between the FNG index and stock prices. Two points in time in particular are of note: the stock-related FNG index sank to a low of 12 on Sept. 17, 2008 after [Lehman Brothers declared bankruptcy](https://www.investopedia.com/articles/economics/09/lehman-brothers-collapse.asp) and AIG nearly closed as well. At the opposite end of the spectrum, the stock-related FNG traded over 90 in September 2012 in response to a positive global reaction to the US Federal Reserves policies. 

The underlying concern of the fear and greed indexes are volatility, which is measured (as volatility and investor reaction to volatility) by the CBOE Volatility index, established by the Chicago Board Options Exchange in 1993 - also referred to as the VIX. The VIX calculation process has subsequently been refined over time. It ranges from 0 to 40.. anything over 30 indicates extreme fearfulness on the part of investors to the level of volatility. A vix score below 20 indicates a comfort level with market conditions.  

This modeling was done in two different ways: one model applies FNG indicators, while the other model is restricted to closing price data alone. Both models use Recurrent Neural Networks (RNN's). 

One idea to improve results would be to incude more data.. the FNG index goes back to January of 2018 (and that data was all provided), our dataset for historical prices went back to July 2019. So additional data on historical prices from January 2018 to June 2019 could be added to the analysis. 

Another idea for improving results would be to derive or regain the base data that the FNG was calculated on over the timeframe, and using those 3 data sets, see if those (all 3 together, or price plus volatility, or price plus volume) would have more predictive effectiveness than the FNG itself in relation to price alone. 

Also added a time tracking feature to start being aware of length of time various functions run.

# Technical Notes

Libraries

-- numpy

-- pandas

--hvplot

--tensorflow

--time


# Acknowledgements

I would like to first acknowledge the guidance and teaching of our FinTech Boot Camp Instructor, Garth Mortensen, our Student Success Manager, Angelica Baraona; and the whole team behind the curriculum, the logistics, the whole program. I also found the collective Stack Overflow wisdom essential as ever. In looking further at the Fear and Greed index, I found these articles helpful: [Crypto Fear and Greed Index Explained - India CSR](https://indiacsr.in/crypto-fear-and-greed-index-explained/) and [Crypto 'Fear & Greed' Index Is Latest Talisman for Bitcoin Fans- Crypto fans are turning to an old Wall Street idea as the latest way to justify buying the dip after the recent slump.](https://www.bloomberg.com/news/articles/2021-12-07/crypto-fear-greed-index-is-latest-talisman-for-bitcoin-fans), and [Investopedia](https://www.investopedia.com/terms/f/fear-and-greed-index.asp).  Some other resources that have enriched by ML journey include 'unBusiness Intelligence' by Dr. Barry Devlin, on the origins of big data,  'Advancing into Analytics' by George Mount was helpful review again of the broader analytics landscape. For machine learning itself from another perspective, I liked 'Python Data Science Handbook' by Jake VanderPlas. My other main resource specifically on this projects' coding was 'Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow' by Aurelien Geron. 

