

- CloudKit
- CKModifySubscriptionsOperation
-  subscriptionsToSave 

Instance Property

# subscriptionsToSave

The subscriptions to save to the database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
var subscriptionsToSave: [CKSubscription]? { get set }
```

## Discussion

This property contains the subscriptions that you want to save. Its initial value is the array that you pass to the init(subscriptionsToSave:subscriptionIDsToDelete:) method. Modify this property as necessary before you execute the operation or submit it to a queue. After CloudKit saves the subscriptions, it begins generating push notifications according to their criteria.

## See Also

### Configuring the Modify Subscriptions Operation

var subscriptionIDsToDelete: [CKSubscription.ID]?

The IDs of the subscriptions that you want to delete.

