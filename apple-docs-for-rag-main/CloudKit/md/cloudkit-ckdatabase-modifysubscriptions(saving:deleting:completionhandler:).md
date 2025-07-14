

- CloudKit
- CKDatabase
-  modifySubscriptions(saving:deleting:completionHandler:) 

Instance Method

# modifySubscriptions(saving:deleting:completionHandler:)

Modifies the specified subscriptions and delivers the results to a completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@preconcurrency
func modifySubscriptions(
    saving subscriptionsToSave: [CKSubscription],
    deleting subscriptionIDsToDelete: [CKSubscription.ID],
    completionHandler: @escaping (Result], deleteResults: [CKSubscription.ID : Result]), any Error>) -> Void
)
```

## Parameters 

`subscriptionsToSave`  

The subscriptions to save.

`subscriptionIDsToDelete`  

The identifiers of the subscriptions to permanently delete.

`completionHandler`  

The closure to execute after CloudKit processes the changes.

## Discussion

The completion handler takes a single Result parameter that contains either a tuple, or an error if the request fails. For example, when the network is unavailable or the device doesn’t have an active iCloud account.

When present, the tuple contains the following named elements:

`saveResults`  
A dictionary of saved subscriptions. The dictionary uses the identifiers of the subscriptions you specify in `subscriptionsToSave` as its keys. The value of each key is a Result that contains either the corresponding modified subscription (as it appears on the server), or an error that describes why CloudKit can’t modify that subscription.

`deleteResults`  
A dictionary of deleted subscriptions. The dictionary uses the identifiers you specify in `subscriptionIDsToDelete` as its keys. The value of each key is a Result that contains either Void to indicate a successful deletion, or an error that describes why CloudKit can’t delete that subscription.

For information on a more configurable way to modify subscriptions, see CKModifySubscriptionsOperation.

## See Also

### Modifying Subscriptions

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID]) async throws -> (saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>])

Modifies the specified subscriptions and returns the results to an awaiting caller.

func save(CKSubscription, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Saves a specific subscription.

func deleteSubscription(withID: CKSubscription.ID) async throws -> CKSubscription.ID

Deletes a specific subscription and returns the deleted subscription’s identifier to an awaiting caller.

func delete(withSubscriptionID: CKSubscription.ID, completionHandler: (String?, (any Error)?) -> Void)

Deletes a specific subscription and delivers the deleted subscription’s identifier to a completion handler.

