

- PassKit (Apple Pay and Wallet)
-  PKPaymentMethod 

Class

# PKPaymentMethod

An object that contains information about payment methods.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentMethod
```

## Topics

### Getting the pass

var secureElementPass: PKSecureElementPass?

The accompanying Secure Element pass.

var paymentPass: PKPaymentPass?

The accompanying payment pass.

Deprecated

### Getting the payment method’s attributes

var type: PKPaymentMethodType

A value that represents the card’s type.

enum PKPaymentMethodType

The type of cards available in Apple Pay.

var displayName: String?

A string, suitable for display, that describes the card.

var network: PKPaymentNetwork?

A string, suitable for display, that describes the payment network for the card.

var billingAddress: CNContact?

The user’s billing address.

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

### Working with payment tokens

var paymentData: Data

The payment data as a UTF-8 encoded serialization of a JSON dictionary.

var paymentMethod: PKPaymentMethod

Information about the card used in the transaction.

var transactionIdentifier: String

A unique identifier for this payment.

