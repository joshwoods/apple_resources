

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.Status
-  updates 

Type Property

# updates

The asynchronous sequence that emits status information when a subscription’s status changes.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var updates: Product.SubscriptionInfo.Status.Statuses { get }
```

## Mentioned in 

Managing Price Increases for Auto-Renewable Subscriptions

## See Also

### Monitoring subscription status changes

static var all: AsyncStream&lt;(groupID: String, statuses: [Product.SubscriptionInfo.Status])>

struct Statuses

An asynchronous sequence that listens for new subscription status information.

