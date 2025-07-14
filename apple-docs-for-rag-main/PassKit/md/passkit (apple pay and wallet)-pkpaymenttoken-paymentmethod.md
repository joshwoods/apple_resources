

- PassKit (Apple Pay and Wallet)
- PKPaymentToken
-  paymentMethod 

Instance Property

# paymentMethod

Information about the card used in the transaction.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var paymentMethod: PKPaymentMethod { get }
```

## See Also

### Working with payment tokens

var paymentData: Data

The payment data as a UTF-8 encoded serialization of a JSON dictionary.

class PKPaymentMethod

An object that contains information about payment methods.

var transactionIdentifier: String

A unique identifier for this payment.

