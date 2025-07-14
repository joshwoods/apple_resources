

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  requiresFelicaSecureElement 

Instance Property

# requiresFelicaSecureElement

A Boolean value that indicates whether the payment pass requires the Felica Secure Element.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var requiresFelicaSecureElement: Bool { get set }
```

## Discussion

This property can be used as a filter to determine which cards are shown in the PKAddPaymentPassViewController class’s intro screen. The property defaults to false.

## See Also

### Filtering pass libraries

var paymentNetwork: PKPaymentNetwork?

The payment network.

var primaryAccountIdentifier: String?

A primary account identifier, used to filter out pass libraries.

