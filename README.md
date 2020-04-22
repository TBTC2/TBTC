# TrakonBTC Public Rest API
The Trackonbtc API can provide the Ticker price API . You can use it to build tickers, price comparison apps, or anything that helps the crypto community. Use it responsibly

## General Information
1. Base API Endpoint: https://trackonbtc.com
1. All public api will return either JSON or Array object.

### Public API Endpoints

1. #### Ticker Price (For All Pairs)
   GET `api/tickerprice`  [Live link](https://api.trackonbtc.com/api/tickerprice)

    > "Ticker Price" will give markets price for all pairs .
    
    ### Response:
    ```
    {"status":200,"message":"ok","data": 
    [
     {"marketPrice":12302.58,"pair":"BTC/AUD","buyrate":12425.6058,"sellrate":12425.6058},
     .....
     {"marketPrice":0.222814,"pair":"XRP/USD","buyrate":0.22504214,"sellrate":0.22504214}
    ]
    }
    ```
     Response has multiple key which denotes market data, this is in JSON. Find all the fields below:
    
    1. `marketPrice`: Market price for this pair
    1. `pair`: Pair symbol
    1. `buyrate`: Buy rate for this pair
    1. `sellrate`: Sell rate for this pair
     
    
2. #### Ticker Price(For Particular Pair)
   GET `/api/tickerprice?pair=BTC/INR` [Live link](https://api.trackonbtc.com/api/tickerprice?pair=BTC/INR)
    > "Ticker Price" will give markets price for particular pair. User can get result for any available pairs .
    
    Returns JSON response which has active market data with all ticker related values.
    ### Response:
    ```
     {"status":200,"message":"ok","data":      
     [{
        "marketPrice":599582,
        "pair":"BTC/INR",
        "buyrate":605577.82,
        "sellrate":605577.82
      }]
     }
    ```
    Response has multiple key which denotes market data, this is in JSON. Find all the fields below:
    
    1. `marketPrice`: Market price for this pair
    1. `pair`: Pair symbol
    1. `buyrate`: Buy rate for this pair
    1. `sellrate`: Sell rate for this pair
         
    
If you have any questions regarding APIs, please reach out to us at mail: support@trackonbtc.com
