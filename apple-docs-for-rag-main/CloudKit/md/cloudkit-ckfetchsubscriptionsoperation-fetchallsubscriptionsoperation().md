

- CloudKit
- CKFetchSubscriptionsOperation
-  fetchAllSubscriptionsOperation() 

Type Method

# fetchAllSubscriptionsOperation()

Returns an operation that fetches all of the user’s subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
class func fetchAllSubscriptionsOperation() -> Self
```

## Discussion

After creating the operation, set the fetchSubscriptionCompletionBlock property to process the results.

