# CFRM-523-ReplicationProjectData

This repository contains the datasets used in my replication paper. The QQQ and TQQQ datasets have slight differences between them, but produce different results so decide how you would like to test the strategy wisely.

The `gaps_removed` datasets skips any days with missing datapoints by removing the data for that day completely.(Method 1)

The `gaps_replaced` datasets will contain data for those days sourced from other data providers such as Alpaca, Bloomberg, AlphaVantage, and other sources. (Method 2)

The `gaps_included` datasets will keep the originally downloaded dataset from Interactive Brokers with missing OHLC candles for certain days. (Method 3)

The `TQQQ_gaps_replaced_atr_extended` dataset contains the data for the 14 trading days occurring before January 4th 2016. This means we included intraday data from December 14th 2015 up until January 4th 2016 in order to calculate the ATR beginning from January 4th 2016. We then filter these days out before running the backtest to ensure we are working with the same days and correctly including the 14 day ATR values.

The datasets containing `_5min_intraday_data` will be the datasets used for our research extension. The dates for the equities are:

1. SPY from January 1st 2017 to February 25th 2025
2. AAPL from January 1st 2017 to February 25th 2025
3. MSTR from January 1st 2019 to February 25th 2025
4. QQQ from January 1st 2019 to February 25th 2025


