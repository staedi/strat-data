# strat-data

This is the repo serving backend data generated for the [Financial News Explorer](https://staedi.github.io/strat-ui).
The original data being generated into this repo is from the financial news, asset prices (price and volume), and SEC EDGAR 10-K financial statement (10-K).

## Types of data

Currently, generated data are the following.

* Topic Clusters (`topics_*.json`): News are being grouped into topic clusters
* Ticker sentiments (`sentiment_*.json`): Each ticker's sentiment (within and out of clusters) is analyzed
* Ticker prices (`prices_*.json`): Each ticker's price data are being gathered
* Company Summary (`company_meta.json`): Summary of company info with its related peers

## Directory structure

### Topic Clusters

* (Root)
  * `topics_recent.json`: Clusters based on recent data
  * `topics_full.json`: Clusters based on full data
  * (topics_weekly)
    * `topics_[YYYY]-W[Week].json`: Clusters of weekly data
   
### Ticker sentiments

* (Root)
  * `sentiment_recent.json`: Ticker sentiments based on recent data
  * `sentiment_full.json`: Ticker sentiments based on full data
  * (sentiment_weekly)
    * `sentiment_[YYYY]-W[Week].json`: Ticker sentiments of weekly data

### Ticker prices

* (Root)
  * `prices_recent.json`: Ticker prices based on recent data
  * `prices_full.json`: Ticker prices based on full data
  * (prices_weekly)
    * `prices_[YYYY]-W[Week].json`: Ticker prices of weekly data

### Company summary

* (Root)
  * `company_meta.json`: (Single) file of Company summary
