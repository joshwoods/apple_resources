

- StoreKit
- Product
-  subscription 

Instance Property

# subscription

The subscription information for an auto-renewable subscripton.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let subscription: Product.SubscriptionInfo?
```

## Discussion

A `nil` value indicates that this product isn’t an auto-renewable subscription.

For more information about subscriptions, see Auto-renewable Subscriptions.

## See Also

### Getting subscription information

struct SubscriptionInfo

Information about an auto-renewable subscription, such as its status, period, subscription group, and subscription offer details.

struct SubscriptionPeriod

Values that represent the duration of time between subscription renewals.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

struct Status

The renewal status information for an auto-renewable subscription.

