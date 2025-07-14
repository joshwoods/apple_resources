

- App Store Server API
-  environment 

Type

# environment

The server environment, either sandbox or production.

App Store Server API 1.0+

``` source
string environment
```

## Possible Values 

`Sandbox`  

Indicates that the data applies to testing in the sandbox environment.

`Production`  

Indicates that the data applies to the production environment.

## Mentioned in 

App Store Server API changelog

## Discussion

You receive data from the App Store Server API for the sandbox environment when you send test requests to the endpoints using the sandbox base URL:

```
```

## See Also

### Response data types

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type hasMore

A Boolean value indicating whether the App Store has more transaction data.

type revision

A token you use in a query to request the next set of transactions for the customer.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

