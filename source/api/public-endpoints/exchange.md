# Exchange

placeholder text

### HTTP Request  
 `GET /v1/exchange/exchangeInfo` <br/>
 Query param (optional):  `market`


Example: `GET /v1/exchange/exchangeInfo?market=INR`

### Response 

> The above command returns JSON structured such as:

```json
{
  "markets": [
    "INR"
  ],
  "contracts": [
    {
      "name": "BTCINR",
      "contractName": "Bitcoin",
      "filters": [
        {
          "maxQty": "120",
          "minQty": "0.001",
          "filterType": "MARKET_QTY_SIZE"
        },
        {
          "maxQty": "1000",
          "minQty": "0.001",
          "filterType": "LIMIT_QTY_SIZE"
        },
        {
          "limit": "200",
          "filterType": "MAX_NUM_ORDERS"
        },
        {
          "notional": "8780",
          "filterType": "MIN_NOTIONAL"
        }
      ],
      "makerFee": 0.005,
      "takerFee": 0.1,
      "baseAsset": "BTC",
      "orderTypes": [
        "LIMIT",
        "MARKET"
      ],
      "quoteAsset": "INR",
      "maxLeverage": "20",
      "contractType": "PERPETUAL",
      "marginBuffer": "0.01",
      "depthGrouping": [
        "0.1"
      ],
      "liquidationFee": "0.020000",
      "pricePrecision": "0",
      "isDefaultContract": true,
      "quantityPrecision": "3",
      "limitPriceVarAllowed": "0.2",
      "marginBufferPercentage": "1",
      "maintenanceMarginPercentage": "1",
      "iconUrl": "string",
      "reduceMarginAllowedRatioPercent": 0.2,
      "market": "INR",
      "marginAssetsSupported": [
        "INR"
      ],
      "fundingFeeInterval": 8
    }
  ],
  "tags": [
    "MEME",
    "DECENTRALIZED"
  ],
  "assetPrecisions": {
    "INR": 2
  },
  "conversionRates": {
    "INR_MARGIN_INR": 1,
    "INR_SETTLEMENT_INR": 1
  }
}
```
