# Market

Fetch the candlestick data for a contract pair.

Available interval values: `1m`, `3m`, `5m`, `15m`, `30m`, `1h`, `2h`, `4h`, `6h`, `8h`, `12h`, `1d`, `3d`, `1w`, `1M`

**m: Minute, h: Hour, d: Day, w: Week, M: Month**

### Klines - HTTP Request

 `POST /v1/market/klines`

```json
{
    "pair": "BTCINR", // Contract Pair
    "interval": "1m", // '1' OR '5' OR '60' OR '1D' for 1min, 5min, 1hour, 1day respectively
    "startTime": 1696425435000, // EPOCH timestamp in milliseconds
    "endTime": 1696425435999, // EPOCH timestamp in milliseconds
    "limit": 1000, // Max limit is 1500 and default limit is 500 if no limit value will be passed
}
```

> The above command returns JSON structured like this:
 
```json
[
 {
    https://github.com/radsatjob/slate
 }

]
```

<aside class="notice">
 The data values will be in descending order of endTime  
</aside>
