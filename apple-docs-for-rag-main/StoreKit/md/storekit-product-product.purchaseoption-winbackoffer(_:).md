

- StoreKit
- Product
- Product.PurchaseOption
-  winBackOffer(\_:) 

Type Method

# winBackOffer(\_:)

Sets a win-back offer to apply to the purchase.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func winBackOffer(_ offer: Product.SubscriptionOffer) -> Product.PurchaseOption
```

## Parameters 

`offer`  

The Product.SubscriptionOffer instance that represents the win-back offer to apply to the purchase.

## Discussion

To test win-back offers in Xcode, set up the offers in your StoreKit configuration file. For more information, see Setting up StoreKit Testing in Xcode.

## See Also

### Setting the purchase options

static func appAccountToken(UUID) -> Product.PurchaseOption

Sets a UUID to associate the purchase with an account in your system.

static func promotionalOffer(offerID: String, keyID: String, nonce: UUID, signature: Data, timestamp: Int) -> Product.PurchaseOption

Applies a promotional offer for an auto-renewable subscription.

static func promotionalOffer(offerID: String, signature: Product.SubscriptionOffer.Signature) -> Product.PurchaseOption

static func quantity(Int) -> Product.PurchaseOption

Indicates the quantity of items the customer is purchasing.

