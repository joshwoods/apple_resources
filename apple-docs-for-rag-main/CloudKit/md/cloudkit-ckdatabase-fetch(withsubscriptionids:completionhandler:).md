

- CloudKit
- CKDatabase
-  fetch(withSubscriptionIDs:completionHandler:) 

Instance Method

# fetch(withSubscriptionIDs:completionHandler:)

Fetches the specified subscriptions and delivers them to a completion handler.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@preconcurrency
func fetch(
    withSubscriptionIDs subscriptionIDs: [CKSubscription.ID],
    completionHandler: @escaping (Result], any Error>) -> Void
)
```

## Parameters 

`subscriptionIDs`  

The identifiers of the subscriptions to fetch.

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- A Result that contains either a dictionary of fetched subscriptions, or an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account. When present, the dictionary uses the identifiers you specify in `subscriptionIDs` as its keys. The value of each key is a Result that contains either the corresponding fetched subscription, or an error that describes why CloudKit can’t provide that subscription.

For information on a more configurable way to fetch specific subscriptions, see CKFetchSubscriptionsOperation.

## See Also

### Fetching Subscriptions

func subscriptions(for: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result&lt;CKSubscription, any Error>]

Fetches the specified subscriptions and returns them to an awaiting caller.

func subscription(for: CKSubscription.ID) async throws -> CKSubscription

Fetches a specific subscription and returns it to an awaiting caller.

func fetch(withSubscriptionID: CKSubscription.ID, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Fetches a specific subscription and delivers it to a completion handler.

func fetchAllSubscriptions(completionHandler: ([CKSubscription]?, (any Error)?) -> Void)

Fetches all subscriptions from the current database.

