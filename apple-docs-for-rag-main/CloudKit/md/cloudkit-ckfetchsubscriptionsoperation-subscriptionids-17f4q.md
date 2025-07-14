

- CloudKit
- CKFetchSubscriptionsOperation
-  subscriptionIDs 

Instance Property

# subscriptionIDs

The IDs of the subscriptions to fetch.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
var subscriptionIDs: [CKSubscription.ID]? { get set }
```

## Discussion

Use this property to view or change the IDs of the subscriptions to fetch. Each element of the array is a string that represents the ID of a subscription. If you intend to modify this property’s value, do so before you execute the operation or submit it to a queue.

If you use the fetchAllSubscriptionsOperation() method to create the operation, CloudKit ignores this property’s value and sets it to `nil`.

