

- CloudKit
- CKFetchSubscriptionsOperation
-  init(subscriptionIDs:) 

Initializer

# init(subscriptionIDs:)

Creates an operation for fetching the specified subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
convenience init(subscriptionIDs: [CKSubscription.ID])
```

## Parameters 

`subscriptionIDs`  

An array of strings where each one is an ID of a subscription that you want to retrieve. This parameter sets the subscriptionIDs property’s value. If you specify `nil`, you must set the `subscriptionIDs` property before you execute the operation.

## Discussion

After creating the operation, assign a closure to the fetchSubscriptionCompletionBlock property to process the results.

## See Also

### Creating a Fetch Subscriptions Operation

init()

Creates an empty fetch subscriptions operation.

