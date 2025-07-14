

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  supportedNetworks 

Instance Property

# supportedNetworks

An array of payment networks the merchant supports.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var supportedNetworks: [PKPaymentNetwork] { get set }
```

## Discussion

This property constrains the selectable payment passes to those the array includes — for example, visa or masterCard.

## See Also

### Setting the merchant information

var merchantIdentifier: String

A string that identifies the merchant.

var merchantCapabilities: PKMerchantCapability

A value that represents the payment-processing capabilities of the merchant.

