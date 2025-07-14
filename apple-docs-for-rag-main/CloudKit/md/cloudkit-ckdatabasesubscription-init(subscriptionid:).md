

- CloudKit
- CKDatabaseSubscription
-  init(subscriptionID:) 

Initializer

# init(subscriptionID:)

Creates a named subscription for all records in a database.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 6.0+Swift 4.2+

``` source
convenience init(subscriptionID: CKSubscription.ID)
```

## Parameters 

`subscriptionID`  

The subscription’s name. It must be unique in the container, and must not be an empty string.

## See Also

### Creating a Database Subscription

convenience init()

Creates an empty database subscription.

Deprecated

init(coder: NSCoder)

Creates a database subscription from a serialized instance.

