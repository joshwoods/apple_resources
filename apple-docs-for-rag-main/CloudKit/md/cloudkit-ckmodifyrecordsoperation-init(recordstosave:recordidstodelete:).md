

- CloudKit
- CKModifyRecordsOperation
-  init(recordsToSave:recordIDsToDelete:) 

Initializer

# init(recordsToSave:recordIDsToDelete:)

Creates an operation for modifying the specified records.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
convenience init(
    recordsToSave: [CKRecord]? = nil,
    recordIDsToDelete: [CKRecord.ID]? = nil
)
```

## Parameters 

`recordsToSave`  

The records to save. You can specify `nil` for this parameter.

`recordIDsToDelete`  

The IDs of the records to delete. You can specify `nil` for this parameter.

## Discussion

The records that you intend to save or delete must all reside in the same database, which you specify when you configure the operation. If your app saves a record in a database that doesn’t exist, the server creates the database.

## See Also

### Creating a Modify Record Operation

init()

Creates an empty modify records operation.

