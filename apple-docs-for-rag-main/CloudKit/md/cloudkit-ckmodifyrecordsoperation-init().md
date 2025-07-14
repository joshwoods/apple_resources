

- CloudKit
- CKModifyRecordsOperation
-  init() 

Initializer

# init()

Creates an empty modify records operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
init()
```

## Discussion

You must set at least one of the recordsToSave or recordIDsToDelete properties before you execute the operation.

## See Also

### Creating a Modify Record Operation

convenience init(recordsToSave: [CKRecord]?, recordIDsToDelete: [CKRecord.ID]?)

Creates an operation for modifying the specified records.

