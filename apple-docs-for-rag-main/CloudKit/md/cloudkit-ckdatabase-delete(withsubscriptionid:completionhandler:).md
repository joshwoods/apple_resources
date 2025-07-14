

- CloudKit
- CKDatabase
-  delete(withSubscriptionID:completionHandler:) 

Instance Method

# delete(withSubscriptionID:completionHandler:)

Deletes a specific subscription and delivers the deleted subscription’s identifier to a completion handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
@preconcurrency
func delete(
    withSubscriptionID subscriptionID: CKSubscription.ID,
    completionHandler: @escaping (String?, (any Error)?) -> Void
)
```

## Parameters 

`subscriptionID`  

The identifier of the subscription to delete.

`completionHandler`  

The closure to execute after CloudKit deletes the subscription.

## Discussion

The completion handler takes the following parameters:

- The identifier of the deleted subscription, or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully deletes the subscription.

For information on a more convenient way to delete subscriptions, see modifySubscriptions(saving:deleting:).

## See Also

### Modifying Subscriptions

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID]) async throws -> (saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>])

Modifies the specified subscriptions and returns the results to an awaiting caller.

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID], completionHandler: (Result&lt;(saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified subscriptions and delivers the results to a completion handler.

func save(CKSubscription, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Saves a specific subscription.

func deleteSubscription(withID: CKSubscription.ID) async throws -> CKSubscription.ID

Deletes a specific subscription and returns the deleted subscription’s identifier to an awaiting caller.

