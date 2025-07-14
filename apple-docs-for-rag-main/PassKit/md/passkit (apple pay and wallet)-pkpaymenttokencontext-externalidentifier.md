

- PassKit (Apple Pay and Wallet)
- PKPaymentTokenContext
-  externalIdentifier 

Instance Property

# externalIdentifier

An external identifier for the merchant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var externalIdentifier: String { get set }
```

## Discussion

An external identifier for the merchant that the app developer provides. If you request a payment token for another merchant, always use the same external identifier for that merchant in your app.

## See Also

### Specifying the merchant

var merchantIdentifier: String

The Apply Pay merchant identifier.

var merchantDomain: String?

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

var merchantName: String

The merchant’s display name that the Apple Pay server associates with the payment token.

