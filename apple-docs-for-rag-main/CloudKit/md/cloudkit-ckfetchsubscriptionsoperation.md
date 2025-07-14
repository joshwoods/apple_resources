

- CloudKit
-  CKFetchSubscriptionsOperation 

Class

# CKFetchSubscriptionsOperation

An operation for fetching subscriptions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
class CKFetchSubscriptionsOperation
```

## Overview

A fetch subscriptions operation retrieves subscriptions (with IDs you already know) from iCloud and can fetch all subscriptions for the current user.

You might fetch subscriptions so you can examine or modify their parameters — for example, to adjust the delivery options for push notifications that the subscription generates.

If you assign a handler to the completionBlock property, the operation calls it after it executes and passes it the results. Use the handler to perform any housekeeping tasks for the operation. The handler you specify should manage any failures, whether due to an error or an explicit cancellation.

## Topics

### Creating a Fetch Subscriptions Operation

convenience init(subscriptionIDs: [CKSubscription.ID])

Creates an operation for fetching the specified subscriptions.

init()

Creates an empty fetch subscriptions operation.

### Getting All Subscriptions

class func fetchAllSubscriptionsOperation() -> Self

Returns an operation that fetches all of the user’s subscriptions.

### Configuring the Fetch Subscriptions Operation

var subscriptionIDs: [CKSubscription.ID]?

The IDs of the subscriptions to fetch.

### Processing the Fetch Subscription Results

var fetchSubscriptionCompletionBlock: (([CKSubscription.ID : CKSubscription]?, (any Error)?) -> Void)?

The block to execute with the fetch results.

### Instance Properties

var fetchSubscriptionsResultBlock: ((Result&lt;Void, any Error>) -> Void)?

var perSubscriptionResultBlock: ((CKSubscription.ID, Result&lt;CKSubscription, any Error>) -> Void)?

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

class CKModifySubscriptionsOperation

An operation for modifying one or more subscriptions.

