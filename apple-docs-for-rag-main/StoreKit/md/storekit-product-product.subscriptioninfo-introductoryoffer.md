

- StoreKit
- Product
- Product.SubscriptionInfo
-  introductoryOffer 

Instance Property

# introductoryOffer

Information about the introductory offer available for the auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let introductoryOffer: Product.SubscriptionOffer?
```

## Discussion

This value is `nil` if you don’t set up an introductory offer in App Store Connect. Use isEligibleForIntroOffer to determine whether the customer is eligible for an introductory offer.

## See Also

### Getting introductory offer details

var isEligibleForIntroOffer: Bool

A Boolean value that indicates whether the customer is eligible for an introductory offer.

static func isEligibleForIntroOffer(for: String) async -> Bool

Returns a Boolean value that determines the customer’s eligibility for an introductory offer within the provided subscription group.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

