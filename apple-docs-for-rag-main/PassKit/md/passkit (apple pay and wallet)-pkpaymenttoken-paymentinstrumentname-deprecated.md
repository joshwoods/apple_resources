

- PassKit (Apple Pay and Wallet)
- PKPaymentToken
-  paymentInstrumentName Deprecated

Instance Property

# paymentInstrumentName

A description of the payment card that the user selected to fund the transaction.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 11.0+visionOS 1.0–1.0Deprecated

``` source
var paymentInstrumentName: String { get }
```

Deprecated

This property is deprecated. Use paymentMethod instead.

## Discussion

This string is suitable for display; it doesn’t contain the full payment information.

## See Also

### Deprecated

var paymentNetwork: String

The payment network for the card that funds this transaction.

Deprecated

