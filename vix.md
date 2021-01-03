# VIX

tag: finance

VIX is the ticker symbol for the Chicago Board Options Exchange (CBOE) Volatility Index, which shows the market's 
expectation of 30-day volatility. It is constructed using the implied volatilities of a wide range of S&P 500 index 
options. This volatility is meant to be forward looking, is calculated from both calls and puts, and is a widely used 
measure of market risk, often referred to as the "investor fear gauge"

VIX values greater than 30 are generally associated with a large amount of volatility as a result of investor fear or 
uncertainty, while values below 20 generally correspond to less stressful, even complacent, times in the markets

## download historical data from cboe

```r
url_vix = "https://ww2.cboe.com/publish/scheduledtask/mktdata/datahouse/vixcurrent.csv"
vix = readr::read_csv(url_vix)
```

## download historical data from yahoo

```r
library("tidyquant")
vix = tq_get("^VIX", from = "2019-01-01")
```

## download historical data from fred

```r
vix1 = q_get("VIXCLS", 
              get = "economic.data",
              from = "2019-01-01")
```

