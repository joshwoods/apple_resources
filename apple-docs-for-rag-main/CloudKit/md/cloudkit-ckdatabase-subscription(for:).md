

- CloudKit
- CKDatabase
-  subscription(for:) 

Instance Method

# subscription(for:)

Fetches a specific subscription and returns it to an awaiting caller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func subscription(for subscriptionID: CKSubscription.ID) async throws -> CKSubscription
```

## Parameters 

`subscriptionID`  

The identifier of the subscription to fetch.

## Return Value

The fetched subscription.

## Discussion

This method throws an error if the request fails, such as when the network is unavailable or the device doesn’t have an active iCloud account.

## See Also

### Fetching Subscriptions

func subscriptions(for: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result&lt;CKSubscription, any Error>]

Fetches the specified subscriptions and returns them to an awaiting caller.

func fetch(withSubscriptionIDs: [CKSubscription.ID], completionHandler: (Result&lt;[CKSubscription.ID : Result&lt;CKSubscription, any Error>], any Error>) -> Void)

Fetches the specified subscriptions and delivers them to a completion handler.

func fetch(withSubscriptionID: CKSubscription.ID, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Fetches a specific subscription and delivers it to a completion handler.

func fetchAllSubscriptions(completionHandler: ([CKSubscription]?, (any Error)?) -> Void)

Fetches all subscriptions from the current database.

