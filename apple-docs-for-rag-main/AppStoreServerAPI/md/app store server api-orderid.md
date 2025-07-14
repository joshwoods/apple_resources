

- App Store Server API
-  orderId 

Type

# orderId

The customer’s order ID from an App Store receipt for in-app purchases.

App Store Server API 1.1+

``` source
string orderId
```

## Discussion

When customers make one or more in-app purchases in your app, the App Store emails them a receipt. The receipt contains an order ID. Use this order ID to call Look Up Order ID. Customers can also retrieve their order IDs from their purchase history on the App Store; for more information, see See your purchase history for the App Store, iTunes store, and more.

## See Also

### Order ID lookup

Look Up Order ID

Get a customer’s in-app purchases from a receipt using the order ID.

object OrderLookupResponse

A response that includes the order lookup status and an array of signed transactions for the in-app purchases in the order.

