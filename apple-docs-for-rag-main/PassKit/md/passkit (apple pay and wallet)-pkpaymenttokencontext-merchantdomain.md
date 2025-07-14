

- PassKit (Apple Pay and Wallet)
- PKPaymentTokenContext
-  merchantDomain 

Instance Property

# merchantDomain

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var merchantDomain: String? { get set }
```

## Discussion

This value is optional; provide the top-level domain for the merchant if it’s available.

## See Also

### Specifying the merchant

var merchantIdentifier: String

The Apply Pay merchant identifier.

var merchantName: String

The merchant’s display name that the Apple Pay server associates with the payment token.

var externalIdentifier: String

An external identifier for the merchant.

