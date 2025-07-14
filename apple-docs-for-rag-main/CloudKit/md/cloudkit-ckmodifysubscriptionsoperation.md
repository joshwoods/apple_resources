

- CloudKit
-  CKModifySubscriptionsOperation 

Class

# CKModifySubscriptionsOperation

An operation for modifying one or more subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
class CKModifySubscriptionsOperation
```

## Overview

After you create or change the configuration of a subscription, use this operation to save those changes to the server. You can also use this operation to permanently delete subscriptions.

If you assign a handler to the completionBlock property, the operation calls it after it executes and passes it the results. Use the handler to perform any housekeeping tasks for the operation. The handler you specify should manage any failures, whether due to an error or an explicit cancellation.

## Topics

### Creating a Modify Subscriptions Operation

convenience init(subscriptionsToSave: [CKSubscription]?, subscriptionIDsToDelete: [CKSubscription.ID]?)

Creates an operation for saving and deleting the specified subscriptions.

init()

Creates an empty modify subscriptions operation.

### Configuring the Modify Subscriptions Operation

var subscriptionsToSave: [CKSubscription]?

The subscriptions to save to the database.

var subscriptionIDsToDelete: [CKSubscription.ID]?

The IDs of the subscriptions that you want to delete.

### Processing the Modify Subscription Results

var modifySubscriptionsCompletionBlock: (([CKSubscription]?, [CKSubscription.ID]?, (any Error)?) -> Void)?

The closure to execute after the operation modifies the subscriptions.

Deprecated

### Instance Properties

var modifySubscriptionsResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perSubscriptionDeleteBlock: ((CKSubscription.ID, Result&lt;Void, any Error>) -> Void)?

var perSubscriptionSaveBlock: ((CKSubscription.ID, Result&lt;CKSubscription, any Error>) -> Void)?

## Relationships

### Inherits From

- CKDatabaseOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Subscription Management

class CKFetchSubscriptionsOperation

An operation for fetching subscriptions.

