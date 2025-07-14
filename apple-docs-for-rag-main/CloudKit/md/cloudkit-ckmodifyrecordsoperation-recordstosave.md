

- CloudKit
- CKModifyRecordsOperation
-  recordsToSave 

Instance Property

# recordsToSave

The records to save to the database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var recordsToSave: [CKRecord]? { get set }
```

## Discussion

The initial value of the property is the array that you provide to the initWithRecordsToSave:recordIDsToDelete: method. You can modify this array as necessary before you execute the operation. The records must all target the same database, but can belong to different record zones.

If you intend to change the value of this property, do so before you execute the operation or submit the operation to a queue.

## See Also

### Configuring the Modify Record Operation

var recordIDsToDelete: [CKRecord.ID]?

The IDs of the records to delete permanently from the database.

var clientChangeTokenData: Data?

A token that tracks local changes to records.

var isAtomic: Bool

A Boolean value that indicates whether the entire operation fails when CloudKit can’t update one or more records in a record zone.

var savePolicy: CKModifyRecordsOperation.RecordSavePolicy

The policy to use when saving changes to records.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

