

- CloudKit
- CKModifySubscriptionsOperation
-  init(subscriptionsToSave:subscriptionIDsToDelete:) 

Initializer

# init(subscriptionsToSave:subscriptionIDsToDelete:)

Creates an operation for saving and deleting the specified subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
convenience init(
    subscriptionsToSave: [CKSubscription]? = nil,
    subscriptionIDsToDelete: [CKSubscription.ID]? = nil
)
```

## Parameters 

`subscriptionsToSave`  

The subscriptions to save or update. You can specify `nil` for this parameter.

`subscriptionIDsToDelete`  

The IDs of the subscriptions to delete. You can specify `nil` for this parameter.

## Discussion

The subscriptions that you want to save or delete must reside in the same container. CloudKit creates a subscription if you save one that doesn’t already exist. CloudKit returns an error if you try to delete a subscription that doesn’t exist.

## See Also

### Creating a Modify Subscriptions Operation

init()

Creates an empty modify subscriptions operation.

