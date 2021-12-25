# DeepLrn-Unit-14-hw11
Deep Learning applied to Bitcoin 



![Deep Learning](Images/deep-learning.jpg)

Enclosed please find two Jupyter Lab notebooks, each modeling bitcoin closing prices using Recurrent Neural Networks (RNN's).  This modeling was done in two different ways: one model applies FNG indicators, while the other model is restricted to closing price data alone. 

FNG (Fear and Greed) indictors relate to the [Crypto Fear and Greed Index (FNG)](https://alternative.me/crypto/fear-and-greed-index/), which ranges from 0 (“Extreme Fear”) to 100 (“Extreme Greed”); and is currently in the 'Fear' zone.

[FNG Index Dial](![image](https://user-images.githubusercontent.com/90283165/147389087-aa8dd046-8aa0-4305-b830-5848fc2b517f.png)

That index is based on three factors:

[]Price changes in major cryptocurrencies (bitcoin, ethereum, and ripple). The larger the change in price, the more important that this data becomes;

[]Volume for each of these cryptocurrencies. The greater the volume, the more important that this data becomes;

[]Volatility. This means how much a cryptocurrency fluctuates in price over time.

This modeling was done in two different ways: one model applies FNG indicators, while the other model is restricted to closing price data alone. Both models use Recurrent Neural Networks (RNN's). 

Also added a time tracking feature to start being aware of length of time various functions run.

# Technical Notes

Libraries

-- numpy

-- pandas

--hvplot

--tensorflow

--time


# Acknowledgements

I would like to first acknowledge the guidance and teaching of our FinTech Boot Camp Instructor, Garth Mortensen, our Student Success Manager, Angelica Baraona; and the whole team behind the curriculum, the logistics, the whole program. I also found the collective Stack Overflow wisdom essential as ever. In looking further at the Fear and Greed index, I found these articles helpful: [Crypto Fear and Greed Index Explained - India CSR](https://indiacsr.in/crypto-fear-and-greed-index-explained/) and [Crypto 'Fear & Greed' Index Is Latest Talisman for Bitcoin Fans- Crypto fans are turning to an old Wall Street idea as the latest way to justify buying the dip after the recent slump.](https://www.bloomberg.com/news/articles/2021-12-07/crypto-fear-greed-index-is-latest-talisman-for-bitcoin-fans).  My other available resource was 'Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow' by Aurelien Geron. 

