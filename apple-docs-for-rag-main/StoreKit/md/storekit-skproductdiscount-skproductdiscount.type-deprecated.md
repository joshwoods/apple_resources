

- StoreKit
- SKProductDiscount
-  SKProductDiscount.Type Deprecated

Enumeration

# SKProductDiscount.Type

Values representing the types of discount offers an app can present.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
enum `Type`
```

Deprecated

Use Product.SubscriptionOffer.OfferType

## Topics

### Types of Offers

case introductory

A constant indicating the discount type is an introductory offer.

case subscription

A constant indicating the discount type is a promotional offer.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the Discount

var identifier: String?

A string used to uniquely identify a discount offer for a product.

Deprecated

var type: SKProductDiscount.Type

The type of discount offer.

Deprecated

