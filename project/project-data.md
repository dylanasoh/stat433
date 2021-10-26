project-data
================
Dylan Asoh
10/26/2021

## Dylan Asoh, Levi Sands, Abdoul Diop

This data set measures the historic open, high, close, trading volume,
and market cap info for a lot of popular crypto currencies.

<https://www.kaggle.com/jessevent/all-crypto-currencies?ref=hackernoon.com>

``` r
df <- read_csv("crypto-markets.csv")
```

    ## Rows: 942297 Columns: 13

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (3): slug, symbol, name
    ## dbl  (9): ranknow, open, high, low, close, volume, market, close_ratio, spread
    ## date (1): date

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
head(df)
```

    ## # A tibble: 6 × 13
    ##   slug    symbol name    date       ranknow  open  high   low close volume market
    ##   <chr>   <chr>  <chr>   <date>       <dbl> <dbl> <dbl> <dbl> <dbl>  <dbl>  <dbl>
    ## 1 bitcoin BTC    Bitcoin 2013-04-28       1  135.  136. 132.  134.       0 1.49e9
    ## 2 bitcoin BTC    Bitcoin 2013-04-29       1  134.  147. 134   145.       0 1.60e9
    ## 3 bitcoin BTC    Bitcoin 2013-04-30       1  144   147. 134.  139        0 1.54e9
    ## 4 bitcoin BTC    Bitcoin 2013-05-01       1  139   140. 108.  117.       0 1.30e9
    ## 5 bitcoin BTC    Bitcoin 2013-05-02       1  116.  126.  92.3 105.       0 1.17e9
    ## 6 bitcoin BTC    Bitcoin 2013-05-03       1  106.  108.  79.1  97.8      0 1.09e9
    ## # … with 2 more variables: close_ratio <dbl>, spread <dbl>
