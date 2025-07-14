

- CloudKit
- CKDatabase
-  subscriptions(for:) 

Instance Method

# subscriptions(for:)

Fetches the specified subscriptions and returns them to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func subscriptions(for ids: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result]
```

## Parameters 

`ids`  

The identifiers of the subscriptions to fetch.

## Return Value

A dictionary that contains the fetched subscriptions. The dictionary uses the identifiers you specify in `ids` as its keys. The value of each key is a Result that contains either the corresponding fetched subscription, or an error that describes why CloudKit can’t provide that subscription.

## Discussion

This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account; otherwise, the returned dictionary includes any individual subscription errors.

For information on a more configurable way to fetch specific subscriptions, see CKFetchSubscriptionsOperation.

## See Also

### Fetching Subscriptions

func fetch(withSubscriptionIDs: [CKSubscription.ID], completionHandler: (Result&lt;[CKSubscription.ID : Result&lt;CKSubscription, any Error>], any Error>) -> Void)

Fetches the specified subscriptions and delivers them to a completion handler.

func subscription(for: CKSubscription.ID) async throws -> CKSubscription

Fetches a specific subscription and returns it to an awaiting caller.

func fetch(withSubscriptionID: CKSubscription.ID, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Fetches a specific subscription and delivers it to a completion handler.

func fetchAllSubscriptions(completionHandler: ([CKSubscription]?, (any Error)?) -> Void)

Fetches all subscriptions from the current database.

