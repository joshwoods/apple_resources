

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassRequestConfiguration
-  paymentNetwork 

Instance Property

# paymentNetwork

The payment network.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
var paymentNetwork: PKPaymentNetwork? { get set }
```

## Discussion

This property determines which cards are shown in the PKAddPaymentPassViewController class’s intro screen. The property defaults to `nil`, and the PKAddPaymentPassViewController shows all the networks for the card’s region. To specify a single network, assign a constant to the property. See Payment Networks in PKPaymentRequest.

## See Also

### Filtering pass libraries

var primaryAccountIdentifier: String?

A primary account identifier, used to filter out pass libraries.

var requiresFelicaSecureElement: Bool

A Boolean value that indicates whether the payment pass requires the Felica Secure Element.

