

- PassKit (Apple Pay and Wallet)
-  PKPaymentToken 

Class

# PKPaymentToken

Contains the user’s payment credentials.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentToken
```

## Overview

You access the payment token for an authorized payment request using the token property of PKPayment.

## Topics

### Working with payment tokens

var paymentData: Data

The payment data as a UTF-8 encoded serialization of a JSON dictionary.

var paymentMethod: PKPaymentMethod

Information about the card used in the transaction.

class PKPaymentMethod

An object that contains information about payment methods.

var transactionIdentifier: String

A unique identifier for this payment.

### Deprecated

var paymentNetwork: String

The payment network for the card that funds this transaction.

Deprecated

var paymentInstrumentName: String

A description of the payment card that the user selected to fund the transaction.

Deprecated

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

### Working with the payment token

var token: PKPaymentToken

The encrypted payment information.

