# TrakonBTC Public Rest API
The Trackonbtc API Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. 

## General Information
1. Base API Endpoint: https://trackonbtc.com
1. All public api will return either JSON or Array object.

### Public API Endpoints

1. #### Ticker Price
   GET `api/tickerprice`  [Live link](https://api.trackonbtc.com/api/tickerprice)

    > "Ticker Price" will give markets price for all pairs .
    
    ### Response:
    ```
    {"status":200,"message":"","data": 
    [
     {"marketPrice":12302.58,"pair":"BTC/AUD","buyrate":12425.6058,"sellrate":12425.6058},
     .....
     {"marketPrice":0.222814,"pair":"XRP/USD","buyrate":0.22504214,"sellrate":0.22504214}
    ]
    }
    ```
     
    
2. #### Ticker Price
   GET `/api/v2/tickerprice?pair=BTC/INR` [Live link](https://api.trackonbtc.com/api/tickerprice?pair=BTC/INR)
    > "Ticker Price" will give markets price for particular pair.
    
    Returns JSON response which has active market data with all ticker related values.
    ### Response:
    ```
     {"status":200,"message":"","data":      
     [{
        "marketPrice":599582,
        "pair":"BTC/INR",
        "buyrate":605577.82,
        "sellrate":605577.82
      }]
     }
    ```
         
    
If you have any questions regarding APIs, please reach out to us at http:/support@trackonbtc.com
