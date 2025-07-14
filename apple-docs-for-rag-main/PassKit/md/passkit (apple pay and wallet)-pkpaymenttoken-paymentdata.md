

- PassKit (Apple Pay and Wallet)
- PKPaymentToken
-  paymentData 

Instance Property

# paymentData

The payment data as a UTF-8 encoded serialization of a JSON dictionary.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var paymentData: Data { get }
```

## Discussion

Send this data to your e-commerce back-end system, where it can be decrypted and submitted to your payment processor.

For the format of the payment data, see Payment Token Format Reference.

## See Also

### Related Documentation

Wallet Developer Guide

### Working with payment tokens

var paymentMethod: PKPaymentMethod

Information about the card used in the transaction.

class PKPaymentMethod

An object that contains information about payment methods.

var transactionIdentifier: String

A unique identifier for this payment.

