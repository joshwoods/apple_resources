

- CloudKit
- CKDatabase
-  deleteSubscription(withID:) 

Instance Method

# deleteSubscription(withID:)

Deletes a specific subscription and returns the deleted subscription’s identifier to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@discardableResult
func deleteSubscription(withID subscriptionID: CKSubscription.ID) async throws -> CKSubscription.ID
```

## Parameters 

`subscriptionID`  

The identifier of the subscription to delete.

## Return Value

The identifier of the deleted subscription.

## Discussion

This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account.

For information on a more convenient way to delete subscriptions, see modifySubscriptions(saving:deleting:).

## See Also

### Modifying Subscriptions

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID]) async throws -> (saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>])

Modifies the specified subscriptions and returns the results to an awaiting caller.

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID], completionHandler: (Result&lt;(saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified subscriptions and delivers the results to a completion handler.

func save(CKSubscription, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Saves a specific subscription.

func delete(withSubscriptionID: CKSubscription.ID, completionHandler: (String?, (any Error)?) -> Void)

Deletes a specific subscription and delivers the deleted subscription’s identifier to a completion handler.

