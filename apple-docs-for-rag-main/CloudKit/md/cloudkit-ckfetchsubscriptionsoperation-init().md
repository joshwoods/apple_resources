

- CloudKit
- CKFetchSubscriptionsOperation
-  init() 

Initializer

# init()

Creates an empty fetch subscriptions operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
init()
```

## Discussion

You must set the subscriptionIDs property before you execute the operation.

## See Also

### Creating a Fetch Subscriptions Operation

convenience init(subscriptionIDs: [CKSubscription.ID])

Creates an operation for fetching the specified subscriptions.

