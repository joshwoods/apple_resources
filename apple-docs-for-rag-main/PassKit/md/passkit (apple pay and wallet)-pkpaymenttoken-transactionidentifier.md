

- PassKit (Apple Pay and Wallet)
- PKPaymentToken
-  transactionIdentifier 

Instance Property

# transactionIdentifier

A unique identifier for this payment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var transactionIdentifier: String { get }
```

## Discussion

This identifier is suitable for use in a receipt.

## See Also

### Working with payment tokens

var paymentData: Data

The payment data as a UTF-8 encoded serialization of a JSON dictionary.

var paymentMethod: PKPaymentMethod

Information about the card used in the transaction.

class PKPaymentMethod

An object that contains information about payment methods.

