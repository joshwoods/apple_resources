

- PassKit (Apple Pay and Wallet)
- PKPaymentToken
-  paymentNetwork Deprecated

Instance Property

# paymentNetwork

The payment network for the card that funds this transaction.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

``` source
var paymentNetwork: String { get }
```

Deprecated

This property is deprecated. Use paymentMethod instead.

## Discussion

The value of this property is one of the constants listed in PKPaymentRequest.

## See Also

### Deprecated

var paymentInstrumentName: String

A description of the payment card that the user selected to fund the transaction.

Deprecated

