

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.Status
-  Product.SubscriptionInfo.Status.Statuses 

Structure

# Product.SubscriptionInfo.Status.Statuses

An asynchronous sequence that listens for new subscription status information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Statuses
```

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Monitoring subscription status changes

static var updates: Product.SubscriptionInfo.Status.Statuses

The asynchronous sequence that emits status information when a subscription’s status changes.

static var all: AsyncStream&lt;(groupID: String, statuses: [Product.SubscriptionInfo.Status])>

