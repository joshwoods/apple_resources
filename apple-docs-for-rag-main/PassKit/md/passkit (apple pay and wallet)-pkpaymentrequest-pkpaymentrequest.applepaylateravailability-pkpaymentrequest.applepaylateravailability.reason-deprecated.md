

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
- PKPaymentRequest.ApplePayLaterAvailability
-  PKPaymentRequest.ApplePayLaterAvailability.Reason Deprecated

Enumeration

# PKPaymentRequest.ApplePayLaterAvailability.Reason

Values you use to enable or disable Apple Pay Later for a specific transaction.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOSwatchOS

``` source
enum Reason
```

Deprecated

Apple Pay Later is deprecated.

## Topics

### Reasons

case itemIneligible

Apple Pay Later is unavailable because one or more ineligible or prohibited items are in the shopping cart, such as gift cards.

case recurringTransaction

Apple Pay Later is unavailable because there’s a recurring payment or subscription in the shopping cart.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

