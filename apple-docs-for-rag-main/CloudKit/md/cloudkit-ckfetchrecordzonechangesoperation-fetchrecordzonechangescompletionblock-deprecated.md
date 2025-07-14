

- CloudKit
- CKFetchRecordZoneChangesOperation
-  fetchRecordZoneChangesCompletionBlock Deprecated

Instance Property

# fetchRecordZoneChangesCompletionBlock

The closure to execute when the operation finishes.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var fetchRecordZoneChangesCompletionBlock: (((any Error)?) -> Void)? { get set }
```

Deprecated

Use fetchRecordZoneChangesResultBlock instead

## Discussion

The closure has no return value and takes the following parameter:

- An error object that contains information about a problem, or `nil` if CloudKit successfully retrieves the record zone changes.

## See Also

### Processing the Zone Change Operation Results

var recordChangedBlock: ((CKRecord) -> Void)?

The closure to execute with the contents of a changed record.

Deprecated

var recordWithIDWasDeletedBlock: ((CKRecord.ID, CKRecord.RecordType) -> Void)?

The closure to execute when a record no longer exists.

var recordZoneChangeTokensUpdatedBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?) -> Void)?

The closure to execute when the change token updates.

var recordZoneFetchCompletionBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?, Bool, (any Error)?) -> Void)?

The closure to execute when a record zone’s fetch finishes.

Deprecated

