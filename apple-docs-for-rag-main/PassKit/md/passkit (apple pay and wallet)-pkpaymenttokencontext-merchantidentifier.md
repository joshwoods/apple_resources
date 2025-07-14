

- PassKit (Apple Pay and Wallet)
- PKPaymentTokenContext
-  merchantIdentifier 

Instance Property

# merchantIdentifier

The Apply Pay merchant identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var merchantIdentifier: String { get set }
```

## Discussion

The merchant identifier you provide when you make an Apple Pay payment request. If you request a payment token for another merchant, use their merchant identifier if available. Otherwise, use your own merchant identifier.

For more information about merchant identifiers, see Setting up Apple Pay.

## See Also

### Specifying the merchant

var merchantDomain: String?

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

var merchantName: String

The merchant’s display name that the Apple Pay server associates with the payment token.

var externalIdentifier: String

An external identifier for the merchant.

