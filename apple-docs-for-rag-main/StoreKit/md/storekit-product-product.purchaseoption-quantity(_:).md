

- StoreKit
- Product
- Product.PurchaseOption
-  quantity(\_:) 

Type Method

# quantity(\_:)

Indicates the quantity of items the customer is purchasing.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func quantity(_ quantity: Int) -> Product.PurchaseOption
```

## Parameters 

`quantity`  

The number of items the customer is purchasing.

The default value is 1. The maximum value is 10.

## Return Value

An instance of Product.PurchaseOption to use in purchase(options:).

## Discussion

The quantity applies to consumable in-app purchases and non-renewing subscriptions.

## See Also

### Setting the purchase options

static func appAccountToken(UUID) -> Product.PurchaseOption

Sets a UUID to associate the purchase with an account in your system.

static func winBackOffer(Product.SubscriptionOffer) -> Product.PurchaseOption

Sets a win-back offer to apply to the purchase.

static func promotionalOffer(offerID: String, keyID: String, nonce: UUID, signature: Data, timestamp: Int) -> Product.PurchaseOption

Applies a promotional offer for an auto-renewable subscription.

static func promotionalOffer(offerID: String, signature: Product.SubscriptionOffer.Signature) -> Product.PurchaseOption

