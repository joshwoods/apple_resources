

- CloudKit
- CKSubscription
-  subscriptionID 

Instance Property

# subscriptionID

The subscription’s unique identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
var subscriptionID: CKSubscription.ID { get }
```

## Discussion

This property’s value is the subscription ID that you provide to the `init(recordType:predicate:subscriptionID:options:)` or `init(zoneID:subscriptionID:options:)` methods when you create the subscription. If you use a different method to create the subscription, CloudKit automatically assigns a UUID as the subscription ID.

## See Also

### Accessing the Subscription Metadata

typealias ID

A type that represents a subscription’s identifier.

var subscriptionType: CKSubscription.SubscriptionType

The behavior that a subscription provides.

enum SubscriptionType

Constants that identify a subscription’s behavior.

