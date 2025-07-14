

- CloudKit
- CKQuery
-  init(coder:) 

Initializer

# init(coder:)

Creates an operation group from a serialized instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

The coder to use when deserializing the group.

## See Also

### Creating a Query

convenience init(recordType: CKRecord.RecordType, predicate: NSPredicate)

Creates a query with the specified record type and predicate.

