

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  primaryAccountIdentifier 

Instance Property

# primaryAccountIdentifier

A primary account identifier, used to filter out pass libraries.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var primaryAccountIdentifier: String? { get set }
```

## Discussion

Users may have different passes installed on different paired devices (for example, on an iPhone and an Apple Watch). This property lets you filter out the devices that already contain a matching pass.

## See Also

### Filtering pass libraries

var paymentNetwork: PKPaymentNetwork?

The payment network.

var requiresFelicaSecureElement: Bool

A Boolean value that indicates whether the payment pass requires the Felica Secure Element.

