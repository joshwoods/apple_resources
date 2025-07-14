

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  merchantIdentifier 

Instance Property

# merchantIdentifier

A string that identifies the merchant.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var merchantIdentifier: String { get set }
```

## Discussion

This string needs to match one of the merchant IDs you registered with the Developer Portal or in Xcode, which the Merchant IDs Entitlement specifies in the app’s entitlements. For more information on adding merchant IDs, see Configure Apple Pay (iOS, watchOS).

## See Also

### Setting the merchant information

var merchantCapabilities: PKMerchantCapability

A value that represents the payment-processing capabilities of the merchant.

var supportedNetworks: [PKPaymentNetwork]

An array of payment networks the merchant supports.

