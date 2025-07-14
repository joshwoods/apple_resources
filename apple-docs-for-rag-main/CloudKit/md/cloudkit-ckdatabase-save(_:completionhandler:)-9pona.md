

- CloudKit
- CKDatabase
-  save(\_:completionHandler:) 

Instance Method

# save(\_:completionHandler:)

Saves a specific subscription.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func save(
    _ subscription: CKSubscription,
    completionHandler: @escaping (CKSubscription?, (any Error)?) -> Void
)
```

``` source
func save(_ subscription: CKSubscription) async throws -> CKSubscription
```

## Parameters 

`subscription`  

The subscription to save.

`completionHandler`  

The closure to execute after CloudKit saves the subscription.

## Discussion

The completion handler takes the following parameters:

- The saved subscription (as it appears on the server), or `nil` if there’s an error.

- An error if a problem occurs, or `nil` if CloudKit successfully saves the subscription.

For information on a more convenient way to save subscriptions, see modifySubscriptions(saving:deleting:).

## See Also

### Modifying Subscriptions

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID]) async throws -> (saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>])

Modifies the specified subscriptions and returns the results to an awaiting caller.

func modifySubscriptions(saving: [CKSubscription], deleting: [CKSubscription.ID], completionHandler: (Result&lt;(saveResults: [CKSubscription.ID : Result&lt;CKSubscription, any Error>], deleteResults: [CKSubscription.ID : Result&lt;Void, any Error>]), any Error>) -> Void)

Modifies the specified subscriptions and delivers the results to a completion handler.

func deleteSubscription(withID: CKSubscription.ID) async throws -> CKSubscription.ID

Deletes a specific subscription and returns the deleted subscription’s identifier to an awaiting caller.

func delete(withSubscriptionID: CKSubscription.ID, completionHandler: (String?, (any Error)?) -> Void)

Deletes a specific subscription and delivers the deleted subscription’s identifier to a completion handler.

