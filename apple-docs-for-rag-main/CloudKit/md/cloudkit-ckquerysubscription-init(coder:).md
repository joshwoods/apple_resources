

- CloudKit
- CKQuerySubscription
-  init(coder:) 

Initializer

# init(coder:)

Creates a query-based subscription from a serialized instance.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
init(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The coder for decoding the serialized query subscription.

## See Also

### Creating a Subscription

convenience init(recordType: CKRecord.RecordType, predicate: NSPredicate, subscriptionID: CKSubscription.ID, options: CKQuerySubscription.Options)

Creates a named query-based subscription that queries records of a specific type.

