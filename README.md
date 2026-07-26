# strat-data

This is the repo serving backend data generated for the [Financial News Explorer](https://staedi.github.io/strat-ui).
The original data being generated into this repo is from the financial news, asset prices (price and volume), SEC EDGAR 10-K financial statement (10-K), and economic indicators via [FRED](https://fred.stlouisfed.org/), [European Central Bank](https://www.ecb.europa.eu/home/html/index.en.html), [Bank of England](https://www.bankofengland.co.uk/), and [Bank of Japan](https://www.boj.or.jp/en/).

## Types of data

Currently, generated data are the following.

* Market Briefings (`briefings.json`): Daily market overview including economic and market snapshots and market movers (based on price changes and sentiment changes)
* Topic Clusters (`topics_*.json`): News are being grouped into topic clusters
* Ticker Sentiments (`sentiment_*.json`): Each ticker's sentiment (within and out of clusters) is analyzed
* Ticker Prices (`prices_*.json`): Each ticker's price data are being gathered
* Company Summary (`company_meta.json`): Summary of company info with its related peers

## Directory structure

### Market Briefings

* `briefings.json`: Daily market overview based on recent data

### Topic Clusters

* `topics_recent.json`: Clusters based on recent data
* `topics_full.json`: Clusters based on full data
   
### Ticker Sentiments

* `sentiment_recent.json`: Ticker sentiments based on recent data
* `sentiment_full.json`: Ticker sentiments based on full data

### Ticker Prices

* `prices_recent.json`: Ticker prices based on recent data
* `prices_full.json`: Ticker prices based on full data

### Company Summary

* `company_meta.json`: (Single) file of Company summary
