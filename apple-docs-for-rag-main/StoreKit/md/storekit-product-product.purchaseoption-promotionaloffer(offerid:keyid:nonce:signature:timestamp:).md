

- StoreKit
- Product
- Product.PurchaseOption
-  promotionalOffer(offerID:keyID:nonce:signature:timestamp:) 

Type Method

# promotionalOffer(offerID:keyID:nonce:signature:timestamp:)

Applies a promotional offer for an auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func promotionalOffer(
    offerID: String,
    keyID: String,
    nonce: UUID,
    signature: Data,
    timestamp: Int
) -> Product.PurchaseOption
```

## Parameters 

`offerID`  

The subscription-offer identifier, id.

`keyID`  

The key ID of the subscription key.

`nonce`  

The antireplay value used in the signature. Use lowercase.

`signature`  

The cryptographic signature of the offer parameters, which you generate on your server.

`timestamp`  

The UNIX time, in milliseconds, when you generate the signature.

## Return Value

An instance of Product.PurchaseOption to use in purchase(options:).

## Discussion

For information about `keyID`, `nonce`, `signature`, and `timestamp`, see Generating a signature for promotional offers. If you’re providing an appAccountToken(_:) in the purchase options, you must include that value when you generate the `signature`. Use lowercase for the UUID string representations of the app account token and the `nonce` in the signature.

You can offer a discounted or free period of service for auto-renewable subscriptions on iOS, iPadOS, macOS, and tvOS using promotional offers. Before you can provide promotional offers in your app, you must set up the offers in your App Store Connect account. To configure your offer, see Set up promotional offers for auto-renewable subscriptions.

## See Also

### Setting the purchase options

static func appAccountToken(UUID) -> Product.PurchaseOption

Sets a UUID to associate the purchase with an account in your system.

static func winBackOffer(Product.SubscriptionOffer) -> Product.PurchaseOption

Sets a win-back offer to apply to the purchase.

static func promotionalOffer(offerID: String, signature: Product.SubscriptionOffer.Signature) -> Product.PurchaseOption

static func quantity(Int) -> Product.PurchaseOption

Indicates the quantity of items the customer is purchasing.

