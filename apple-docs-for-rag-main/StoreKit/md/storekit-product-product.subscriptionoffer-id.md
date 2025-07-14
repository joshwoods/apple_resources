

- StoreKit
- Product
- Product.SubscriptionOffer
-  id 

Instance Property

# id

The subscription offer identifier.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let id: String?
```

## Mentioned in 

Merchandising win-back offers in your app

## Discussion

The id is a string that contains the alphanumeric offer identifier you provide when you configure a subscription offer in App Store Connect.

This value is `nil` if the subscription offer is an introductory offer.

Pass the id to a method in purchase(options:) to create a purchase option based on the offer’s type. For example, pass the id for a promotional offer to the promotionalOffer(offerID:signature:) to apply the promotion to a purchase.

For more information about configuring offers in App Store Connect, see Product.SubscriptionOffer.

