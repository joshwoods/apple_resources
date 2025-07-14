

- CloudKit
- CKDatabaseSubscription
-  init(coder:) 

Initializer

# init(coder:)

Creates a database subscription from a serialized instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
init(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The object that decodes the serialized database subscription.

## See Also

### Creating a Database Subscription

convenience init()

Creates an empty database subscription.

Deprecated

convenience init(subscriptionID: CKSubscription.ID)

Creates a named subscription for all records in a database.

