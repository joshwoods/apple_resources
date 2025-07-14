

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  merchantCapabilities 

Instance Property

# merchantCapabilities

A value that represents the payment-processing capabilities of the merchant.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var merchantCapabilities: PKMerchantCapability { get set }
```

## See Also

### Setting the merchant information

var merchantIdentifier: String

A string that identifies the merchant.

var supportedNetworks: [PKPaymentNetwork]

An array of payment networks the merchant supports.

