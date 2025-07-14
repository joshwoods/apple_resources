

- PassKit (Apple Pay and Wallet)
- PKPaymentTokenContext
-  merchantName 

Instance Property

# merchantName

The merchant’s display name that the Apple Pay server associates with the payment token.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var merchantName: String { get set }
```

## Discussion

Provide the name of the merchant associated with the payment token, to display to the user.

## See Also

### Specifying the merchant

var merchantIdentifier: String

The Apply Pay merchant identifier.

var merchantDomain: String?

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

var externalIdentifier: String

An external identifier for the merchant.

