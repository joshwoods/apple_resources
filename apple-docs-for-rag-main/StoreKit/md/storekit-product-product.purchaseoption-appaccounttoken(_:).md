

- StoreKit
- Product
- Product.PurchaseOption
-  appAccountToken(\_:) 

Type Method

# appAccountToken(\_:)

Sets a UUID to associate the purchase with an account in your system.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func appAccountToken(_ token: UUID) -> Product.PurchaseOption
```

## Parameters 

`token`  

A UUID you provide to associate with the purchase.

## Return Value

An instance of Product.PurchaseOption to use in purchase(options:).

## Discussion

When you set the app account token in the purchase options, the App Store returns the same app account token value in the resulting transaction, in appAccountToken.

## See Also

### Setting the purchase options

static func winBackOffer(Product.SubscriptionOffer) -> Product.PurchaseOption

Sets a win-back offer to apply to the purchase.

static func promotionalOffer(offerID: String, keyID: String, nonce: UUID, signature: Data, timestamp: Int) -> Product.PurchaseOption

Applies a promotional offer for an auto-renewable subscription.

static func promotionalOffer(offerID: String, signature: Product.SubscriptionOffer.Signature) -> Product.PurchaseOption

static func quantity(Int) -> Product.PurchaseOption

Indicates the quantity of items the customer is purchasing.

