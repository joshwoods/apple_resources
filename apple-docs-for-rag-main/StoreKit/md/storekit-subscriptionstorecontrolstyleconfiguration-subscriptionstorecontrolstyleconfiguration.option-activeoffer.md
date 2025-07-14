

- StoreKit
- SubscriptionStoreControlStyleConfiguration
- SubscriptionStoreControlStyleConfiguration.Option
-  activeOffer 

Instance Property

# activeOffer

The subscription offer the customer is eligible for, and that applies to the subscription option.

StoreKitSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var activeOffer: Product.SubscriptionOffer? { get }
```

## Discussion

Always display the terms of this subscription offer along with your control because it represents the offer that StoreKit automatically applies when you call the subscribe() method. If the activeOffer property is `nil`, there’s no subscription offer.

Important

Don’t display offers from properties of subscription, such as introductoryOffer.

The preferredSubscriptionOffer(_:) and subscriptionPromotionalOffer(offer:signature:) view modifiers influence the offer property.

## See Also

### Getting the subscription product and offer

var subscription: Product

The auto-renewable subscription to merchandise.

var id: Product.ID

The product ID of the auto-renewable subscription.

