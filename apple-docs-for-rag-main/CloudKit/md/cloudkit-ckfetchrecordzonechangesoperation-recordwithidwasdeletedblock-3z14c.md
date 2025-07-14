

- CloudKit
- CKFetchRecordZoneChangesOperation
-  recordWithIDWasDeletedBlock 

Instance Property

# recordWithIDWasDeletedBlock

The closure to execute when a record no longer exists.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
var recordWithIDWasDeletedBlock: ((CKRecord.ID, CKRecord.RecordType) -> Void)? { get set }
```

## Discussion

The closure returns no value and takes the following parameters:

- The deleted record’s ID.

- The deleted record’s type.

The operation executes this closure once for each record the server deletes after the previous change token. Each time the closure executes, it executes serially with respect to the other closures of the operation. If there aren’t any record deletions, this closure doesn’t execute.

Set this property before you execute the operation or submit it to a queue.

## See Also

### Processing the Zone Change Operation Results

var recordChangedBlock: ((CKRecord) -> Void)?

The closure to execute with the contents of a changed record.

Deprecated

var recordZoneChangeTokensUpdatedBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?) -> Void)?

The closure to execute when the change token updates.

var recordZoneFetchCompletionBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?, Bool, (any Error)?) -> Void)?

The closure to execute when a record zone’s fetch finishes.

Deprecated

var fetchRecordZoneChangesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated

