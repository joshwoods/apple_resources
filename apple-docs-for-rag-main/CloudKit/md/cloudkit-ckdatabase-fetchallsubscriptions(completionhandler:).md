

- CloudKit
- CKDatabase
-  fetchAllSubscriptions(completionHandler:) 

Instance Method

# fetchAllSubscriptions(completionHandler:)

Fetches all subscriptions from the current database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func fetchAllSubscriptions(completionHandler: @escaping ([CKSubscription]?, (any Error)?) -> Void)
```

``` source
func allSubscriptions() async throws -> [CKSubscription]
```

## Parameters 

`completionHandler`  

The closure to execute with the fetch results.

## Discussion

The completion handler takes the following parameters:

- The database’s subscriptions, or `nil` if CloudKit can’t provide the subscriptions.

- An error if a problem occurs, or `nil` if the fetch completes successfully.

For information on a more configurable way to fetch all subscriptions from a specific database, see fetchAllSubscriptionsOperation().

## See Also

### Fetching Subscriptions

func subscriptions(for: [CKSubscription.ID]) async throws -> [CKSubscription.ID : Result&lt;CKSubscription, any Error>]

Fetches the specified subscriptions and returns them to an awaiting caller.

func fetch(withSubscriptionIDs: [CKSubscription.ID], completionHandler: (Result&lt;[CKSubscription.ID : Result&lt;CKSubscription, any Error>], any Error>) -> Void)

Fetches the specified subscriptions and delivers them to a completion handler.

func subscription(for: CKSubscription.ID) async throws -> CKSubscription

Fetches a specific subscription and returns it to an awaiting caller.

func fetch(withSubscriptionID: CKSubscription.ID, completionHandler: (CKSubscription?, (any Error)?) -> Void)

Fetches a specific subscription and delivers it to a completion handler.

