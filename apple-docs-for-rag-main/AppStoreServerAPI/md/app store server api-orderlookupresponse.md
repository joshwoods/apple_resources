

- App Store Server API
-  OrderLookupResponse 

Object

# OrderLookupResponse

A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.

App Store Server API 1.1+

``` source
object OrderLookupResponse
```

## Properties

`status`

OrderLookupStatus

The status that indicates whether the order ID is valid.

`signedTransactions`

`[`JWSTransaction`]`

An array of in-app purchase transactions that are part of order, signed by Apple, in JSON Web Signature format.

## Discussion

The order lookup response contains information about the orderId you specify when you call Look Up Order ID.

If the `orderId` that you provide in the request is invalid, the response doesn’t include the `signedTransactions` array. If the `orderId` is valid, expect at least one transaction in the `signedTransactions` array.

## Topics

### Response data types

type OrderLookupStatus

A value that indicates whether the order ID in the request is valid for your app.

## See Also

### Order ID lookup

Look Up Order ID

Get a customer’s in-app purchases from a receipt using the order ID.

type orderId

The customer’s order ID from an App Store receipt for in-app purchases.

