

- App Store Server API
-  revision 

Type

# revision

A token you use in a query to request the next set of transactions for the customer.

App Store Server API 1.0+

``` source
string revision
```

## Discussion

The App Store server returns a `revision` value in each response to certain endpoints, such as Get Transaction History and Get Refund History. Use the `revision` value to get a set of paginated transactions.

The first time you call an endpoint, you don’t include a `revision` query parameter, and the API returns the customer’s first set of up to 20 transactions. If there are more transactions, the hasMore value in the response is `true`. To get the next set of transactions, use the revision value from the response in your subsequent call to the endpoint.

Consider storing the `revision` value from the last page of transactions, when the hasMore value is `false`, with other customer account information. Use it the next time you call the endpoint for the same customer, to avoid fetching transactions you’ve already received. For the Get Transaction History endpoint, store the `revision` value only if you request the transaction history in `ASCENDING` sort order.

## See Also

### Response data types

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type environment

The server environment, either sandbox or production.

type hasMore

A Boolean value indicating whether the App Store has more transaction data.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

