

- App Store Server API
-  hasMore 

Type

# hasMore

A Boolean value indicating whether the App Store has more transaction data.

App Store Server API 1.0+

``` source
boolean hasMore
```

## Discussion

This value is `true` if the App Store has more transactions for the customer. Call the endpoint again, including the revision or paginationToken query parameter, to get the next set of transactions.

If this value is `false`, there aren’t any additional transactions.

The hasMore value appears in responses to endpoints that provide paginated results, such as NotificationHistoryResponse, HistoryResponse, and RefundHistoryResponse.

## See Also

### Response data types

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type environment

The server environment, either sandbox or production.

type revision

A token you use in a query to request the next set of transactions for the customer.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

