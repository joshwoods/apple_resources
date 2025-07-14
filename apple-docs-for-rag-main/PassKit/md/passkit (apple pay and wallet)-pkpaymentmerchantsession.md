

- PassKit (Apple Pay and Wallet)
-  PKPaymentMerchantSession 

Class

# PKPaymentMerchantSession

An object that validates the identity of a merchant for a payment request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 7.0+

``` source
class PKPaymentMerchantSession
```

## Topics

### Creating a merchant session

init(dictionary: [AnyHashable : Any])

Creates an object that validates the identity of a merchant for a payment request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Getting information for the merchant session update

var status: PKPaymentAuthorizationStatus

The current authorization status for the payment.

var session: PKPaymentMerchantSession?

An object that validates the identity of a merchant for the payment request.

