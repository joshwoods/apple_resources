

- CloudKit
- CKDatabase
-  fetch(withSubscriptionID:completionHandler:) 

Instance Method

# fetch(withSubscriptionID:completionHandler:)

Fetches a specific subscription and delivers it to a completion handler.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
@preconcurrency
func fetch(
    withSubscriptionID subscriptionID: CKSubscription.ID,
    completionHandler: @escaping (CKSubscription?, (any Error)?) -> Void
)
```

## Parameters 

`subscriptionID`  

The identifier of the subscription to fetch.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- The requested subscription, or `nil` if CloudKit can’t provide that subscription.

- An error if a problem occurs, or `nil` if the fetch completes successfully.

For information on a more convenient way to fetch specific subscriptions, see subscriptions(for:).

## See Also

### Fetching Subscriptions

func subscriptions(for: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result&lt;CKSubscription, any Error>]

Fetches the specified subscriptions and returns them to an awaiting caller.

func fetch(withSubscriptionIDs: [CKSubscription.ID], completionHandler: (Result&lt;[CKSubscription.ID : Result&lt;CKSubscription, any Error>], any Error>) -> Void)

Fetches the specified subscriptions and delivers them to a completion handler.

func subscription(for: CKSubscription.ID) async throws -> CKSubscription

Fetches a specific subscription and returns it to an awaiting caller.

func fetchAllSubscriptions(completionHandler: ([CKSubscription]?, (any Error)?) -> Void)

Fetches all subscriptions from the current database.

