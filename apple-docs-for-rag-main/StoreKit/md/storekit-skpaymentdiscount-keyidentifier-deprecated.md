

- StoreKit
- SKPaymentDiscount
-  keyIdentifier Deprecated

Instance Property

# keyIdentifier

A string that identifies the key used to generate the signature.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var keyIdentifier: String { get }
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

## Discussion

You generate and download keys from App Store Connect. See the “KEY ID” column in App Store Connect to use as the keyIdentifier.

## See Also

### Identifying the Discount

var identifier: String

A string used to uniquely identify a discount offer for a product.

Deprecated

