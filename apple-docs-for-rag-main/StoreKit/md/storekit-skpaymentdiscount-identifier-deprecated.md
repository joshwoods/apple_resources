

- StoreKit
- SKPaymentDiscount
-  identifier Deprecated

Instance Property

# identifier

A string used to uniquely identify a discount offer for a product.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var identifier: String { get }
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

## Discussion

You set up offers and their identifiers in App Store Connect. If the identifier is not valid, an SKError.Code.invalidOfferIdentifier error can result.

## See Also

### Identifying the Discount

var keyIdentifier: String

A string that identifies the key used to generate the signature.

Deprecated

