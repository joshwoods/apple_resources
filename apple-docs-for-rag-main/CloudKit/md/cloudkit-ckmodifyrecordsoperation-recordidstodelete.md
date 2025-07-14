

- CloudKit
- CKModifyRecordsOperation
-  recordIDsToDelete 

Instance Property

# recordIDsToDelete

The IDs of the records to delete permanently from the database.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
var recordIDsToDelete: [CKRecord.ID]? { get set }
```

## Discussion

An array of CKRecord.ID objects that identifies the records to delete. The initial value of the property is the array of record IDs that you provide to the initWithRecordsToSave:recordIDsToDelete: method.

When deleting records, the operation reports progress only on the records with the IDs that you specify in this property. Deleting records can trigger the deletion of related records if there is an owner-owned relationship between the records involving a CKRecord.Reference object. When additional deletions occur, CloudKit doesn’t pass them to the progress handler of the operation. For that reason, it’s important to understand the implications of the ownership model you use when you relate records to each other through a CKRecord.Reference object. For more information about owner-owned relationships, see CKRecord.Reference.

If you intend to change the value of this property, do so before you execute the operation or submit the operation to a queue.

## See Also

### Configuring the Modify Record Operation

var recordsToSave: [CKRecord]?

The records to save to the database.

var clientChangeTokenData: Data?

A token that tracks local changes to records.

var isAtomic: Bool

A Boolean value that indicates whether the entire operation fails when CloudKit can’t update one or more records in a record zone.

var savePolicy: CKModifyRecordsOperation.RecordSavePolicy

The policy to use when saving changes to records.

enum RecordSavePolicy

Constants that indicate which policy to apply when saving records.

