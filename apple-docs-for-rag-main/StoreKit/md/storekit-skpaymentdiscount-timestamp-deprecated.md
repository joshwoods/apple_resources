

- StoreKit
- SKPaymentDiscount
-  timestamp Deprecated

Instance Property

# timestamp

The date and time of the signature’s creation in milliseconds, formatted in Unix epoch time.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
@NSCopying
var timestamp: NSNumber { get }
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

## Discussion

The timestamp keeps the payment discount active for 24 hours.

## See Also

### Validating the Discount

var nonce: UUID

A universally unique ID (UUID) value that you define.

Deprecated

var signature: String

A string representing the properties of a specific promotional offer, cryptographically signed.

Deprecated

