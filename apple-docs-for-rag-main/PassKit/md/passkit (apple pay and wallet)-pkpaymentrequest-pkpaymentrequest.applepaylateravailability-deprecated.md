

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  PKPaymentRequest.ApplePayLaterAvailability Deprecated

Enumeration

# PKPaymentRequest.ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+visionOSwatchOS

``` source
enum ApplePayLaterAvailability
```

Deprecated

Apple Pay Later is deprecated.

## Topics

### Availability

case unavailable(PKPaymentRequest.ApplePayLaterAvailability.Reason)

Apple Pay Later is not available.

case available

Apple Pay Later is available.

### Transaction availability reasons

enum Reason

Values you use to enable or disable Apple Pay Later for a specific transaction.

## See Also

### Deprecated

var applePayLaterAvailability: PKPaymentRequest.ApplePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Deprecated

struct PKAddressField

Billing or shipping address fields.

Deprecated

enum PKApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

