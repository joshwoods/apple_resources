

- CloudKit
- CKModifySubscriptionsOperation
-  modifySubscriptionsCompletionBlock Deprecated

Instance Property

# modifySubscriptionsCompletionBlock

The closure to execute after the operation modifies the subscriptions.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOSwatchOS 6.0–8.0Deprecated

``` source
var modifySubscriptionsCompletionBlock: (([CKSubscription]?, [CKSubscription.ID]?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use modifySubscriptionsResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- The subscriptions to save.

- The IDs of the subscriptions to delete.

- An error that contains information about a problem, or `nil` if CloudKit successfully modifies the subscriptions.

The operation executes this closure only once, and it’s your only opportunity to process the results. The closure executes on a background queue, so any tasks that require access to the main queue must dispatch accordingly.

The closure reports an error of type CKError.Code.partialFailure when it can’t modify some of the subscriptions. The userInfo dictionary of the error contains a CKPartialErrorsByItemIDKey key that has a dictionary as its value. The keys of the dictionary are the IDs of the subscriptions that CloudKit can’t modify, and the corresponding values are errors that contain information about the failures.

Set this property’s value before you execute the operation or submit it to a queue.

