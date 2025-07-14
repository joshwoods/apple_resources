

- PassKit (Apple Pay and Wallet)
- PKPaymentRequest
-  merchantCapabilities 

Instance Property

# merchantCapabilities

A bit field of the payment-processing protocols and card types that you support.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var merchantCapabilities: PKMerchantCapability { get set }
```

## Discussion

The threeDSecure and emv values of PKMerchantCapability specify the supported cryptographic payment protocols. At least one of these two values is required.

Check with your payment processors about the cryptographic payment protocols they support. As a general rule, if you want to support China UnionPay cards, you use `capabilityEMV`. To support cards from other networks—like American Express, Visa, or Mastercard—use `capability3DS`.

To filter the types of cards to make available for the transaction, pass the credit and debit values. If neither is passed, all card types will be available.

## See Also

### Setting merchant information

struct MerchantCategoryCode

An optional four-digit struct, in ISO 18245 format, that represents the type of goods or service the merchant provides for the transaction.

var merchantIdentifier: String

Your merchant identifier.

struct PKMerchantCapability

Capabilities for processing payment.

