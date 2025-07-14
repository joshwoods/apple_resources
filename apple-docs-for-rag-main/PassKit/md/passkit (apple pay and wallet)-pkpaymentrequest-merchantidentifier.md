

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  merchantIdentifier 

Instance Property

# merchantIdentifier

Your merchant identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var merchantIdentifier: String { get set }
```

## Discussion

This value must match one of the merchant identifiers specified by the Merchant IDs Entitlement key in the app’s entitlements. For more information on adding merchant IDs, see Configure Apple Pay (iOS, watchOS).

## See Also

### Setting merchant information

struct MerchantCategoryCode

An optional four-digit struct, in ISO 18245 format, that represents the type of goods or service the merchant provides for the transaction.

var merchantCapabilities: PKMerchantCapability

A bit field of the payment-processing protocols and card types that you support.

struct PKMerchantCapability

Capabilities for processing payment.

