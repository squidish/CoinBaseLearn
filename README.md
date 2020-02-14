# CoinBaseLearn
Uses SVM to attempt to learn a profitable trading strategy on Coinbase Pro BTC exchange

## Labelling
 
The code loads data from the Coinbase Pro directory and labels it using the triple barrier method from:  

"Advances in Financial Machine Learning". by Marcos Lopez De Prado  

Where point are labeled true if an investment at this point would produce a retrun above a volatility dependent threshold within a give time without hitting a stop-loss limit.

## SVM

The SVM implementation in SkLearn is used to learn what points will fit this criteon based on the features: Opening Price, Volume, 2d EWMA, 8d EWMA. 
