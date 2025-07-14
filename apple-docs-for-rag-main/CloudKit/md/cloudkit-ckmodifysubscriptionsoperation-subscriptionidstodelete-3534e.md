

- CloudKit
- CKModifySubscriptionsOperation
-  subscriptionIDsToDelete 

Instance Property

# subscriptionIDsToDelete

The IDs of the subscriptions that you want to delete.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
var subscriptionIDsToDelete: [CKSubscription.ID]? { get set }
```

## Discussion

This property contains the IDs of the subscriptions that you want to delete. Its initial value is the array that you pass to the init(subscriptionsToSave:subscriptionIDsToDelete:) method. Modify this property as necessary before you execute the operation or submit it to a queue.

## See Also

### Configuring the Modify Subscriptions Operation

var subscriptionsToSave: [CKSubscription]?

The subscriptions to save to the database.

