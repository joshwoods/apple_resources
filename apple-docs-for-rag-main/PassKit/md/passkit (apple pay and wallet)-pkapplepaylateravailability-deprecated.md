

- PassKit (Apple Pay and Wallet)
-  PKApplePayLaterAvailability Deprecated

Enumeration

# PKApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
enum PKApplePayLaterAvailability
```

Deprecated

Apple Pay Later is deprecated.

## Topics

### Availability values

case available

Apple Pay Later is available.

case unavailableItemIneligible

Apple Pay Later is unavailable because one or more ineligible or prohibited items are in the shopping cart, such as gift cards.

case unavailableRecurringTransaction

Apple Pay Later is unavailable because there’s a recurring payment or subscription in the shopping cart.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

enum ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

