# CFRM-523-ReplicationProjectData

This repository contains 3 seperate datasets for QQQ and TQQQ used in my replication paper. They have slight differences between them, but will produce different results so decide how you would like to test the strategy wisely.

The 'gaps_removed' datasets skips any days with missing datapoints by removing the data for that day completely.(Method 1 and used in the replication paper)

The 'gaps_replaced' datasets will contain data for those days sourced from other data providers such as Alpaca, Bloomberg, AlphaVantage, and other sources. (Method 2)

The `gaps_included` datasets will keep the originally downloaded dataset from Interactive Brokers with missing OHLC candles for certain days. (Method 3)
