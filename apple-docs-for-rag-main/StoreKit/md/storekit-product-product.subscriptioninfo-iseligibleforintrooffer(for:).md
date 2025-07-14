

- StoreKit
- Product
- Product.SubscriptionInfo
-  isEligibleForIntroOffer(for:) 

Type Method

# isEligibleForIntroOffer(for:)

Returns a Boolean value that determines the customer’s eligibility for an introductory offer within the provided subscription group.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func isEligibleForIntroOffer(for groupID: String) async -> Bool
```

## Parameters 

`groupID`  

The subscription group identifier to check eligibility for an introductory offer.

## Return Value

`true` if the customer is eligible for an introductory offer on any auto-renewable subscription within the subscription group; `false` otherwise.

## Discussion

This value may be `true` even if you haven’t set up an introductory offer in App Store Connect.

## See Also

### Getting introductory offer details

var isEligibleForIntroOffer: Bool

A Boolean value that indicates whether the customer is eligible for an introductory offer.

let introductoryOffer: Product.SubscriptionOffer?

Information about the introductory offer available for the auto-renewable subscription.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

