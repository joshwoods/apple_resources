

- CloudKit
- CKFetchRecordZoneChangesOperation
-  recordChangedBlock Deprecated

Instance Property

# recordChangedBlock

The closure to execute with the contents of a changed record.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var recordChangedBlock: ((CKRecord) -> Void)? { get set }
```

Deprecated

Use recordWasChangedBlock instead, which surfaces per-record errors

## Discussion

The closure returns no value and takes the following parameter:

- The changed record. If you specify a value for the desiredKeys property, the record contains only the corresponding fields.

The operation executes this closure once for each record in the record zone with changes since the previous fetch request. Each time the closure executes, it executes serially with respect to the other closures of the operation. If there aren’t any record changes, this closure doesn’t execute.

Set this property before you execute the operation or submit it to a queue.

## See Also

### Processing the Zone Change Operation Results

var recordWithIDWasDeletedBlock: ((CKRecord.ID, CKRecord.RecordType) -> Void)?

The closure to execute when a record no longer exists.

var recordZoneChangeTokensUpdatedBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?) -> Void)?

The closure to execute when the change token updates.

var recordZoneFetchCompletionBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?, Bool, (any Error)?) -> Void)?

The closure to execute when a record zone’s fetch finishes.

Deprecated

var fetchRecordZoneChangesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated

