

- StoreKit Test
- SKTestSession
-  buyProduct(productIdentifier:) Deprecated

Instance Method

# buyProduct(productIdentifier:)

Simulates buying an in-app purchase or subscription outside the app.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedwatchOS 7.0–10.0Deprecated

``` source
func buyProduct(productIdentifier: String) throws
```

Deprecated

Use the Swift API: SKTestSession.buyProduct(identifier:, options:)

## Parameters 

`productIdentifier`  

Product identifier of the in-app purchase.

## Discussion

After calling this function, handle the new transaction in your payment queue.

## See Also

### Testing externally performed transactions

func refundTransaction(identifier: Int) throws

Simulates a refund for an in-app purchase that completes outside of the app.

