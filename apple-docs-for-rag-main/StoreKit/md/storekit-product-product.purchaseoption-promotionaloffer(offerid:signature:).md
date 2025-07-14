

- StoreKit
- Product
- Product.PurchaseOption
-  promotionalOffer(offerID:signature:) 

Type Method

# promotionalOffer(offerID:signature:)

iOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static func promotionalOffer(
    offerID: String,
    signature: Product.SubscriptionOffer.Signature
) -> Product.PurchaseOption
```

## See Also

### Setting the purchase options

static func appAccountToken(UUID) -> Product.PurchaseOption

Sets a UUID to associate the purchase with an account in your system.

static func winBackOffer(Product.SubscriptionOffer) -> Product.PurchaseOption

Sets a win-back offer to apply to the purchase.

static func promotionalOffer(offerID: String, keyID: String, nonce: UUID, signature: Data, timestamp: Int) -> Product.PurchaseOption

Applies a promotional offer for an auto-renewable subscription.

static func quantity(Int) -> Product.PurchaseOption

Indicates the quantity of items the customer is purchasing.

