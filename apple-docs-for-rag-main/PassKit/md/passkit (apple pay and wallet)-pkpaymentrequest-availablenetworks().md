

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  availableNetworks() 

Type Method

# availableNetworks()

Returns the list of available payment methods that Apple Pay supports.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class func availableNetworks() -> [PKPaymentNetwork]
```

## Return Value

An array of strings representing the available payment networks. For a list of possible networks, see PKPaymentNetwork.

## Discussion

To dynamically select the payment networks at runtime, use this method to get the complete list of currently supported networks. You can then filter this list, as needed, and assign the results to the payment request’s supportedNetworks property.

## See Also

### Related Documentation

Wallet Developer Guide

### Selecting the payment networks

var supportedNetworks: [PKPaymentNetwork]

The payment methods that you support.

struct PKPaymentNetwork

A type that represents a payment method.

