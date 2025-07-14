

- CloudKit
- CKFetchRecordZoneChangesOperation
-  recordZoneFetchCompletionBlock Deprecated

Instance Property

# recordZoneFetchCompletionBlock

The closure to execute when a record zone’s fetch finishes.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var recordZoneFetchCompletionBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?, Bool, (any Error)?) -> Void)? { get set }
```

Deprecated

Use recordZoneFetchResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- The record zone’s ID.

- The change token to store and use in subsequent instances of CKFetchRecordZoneChangesOperation.

- The more recent client change token from the device. If the change token isn’t the more recent change token you provided, the server might not have received the associated changes.

- A Boolean that indicates whether this is the final record zone change. If fetchAllChanges is false, it’s the app’s responsibility to create additional instances of CKFetchRecordZoneChangesOperation to fetch further changes.

- An error object that contains information about a problem, or `nil` if the operation successfully retrieves the results.

The app is responsible for saving the change token at the end of the operation and providing it to future uses of CKFetchRecordZoneChangesOperation. Each time the closure executes, it executes serially with respect to the other closures of the operation.

Set this property before you execute the operation or submit it to a queue.

## See Also

### Processing the Zone Change Operation Results

var recordChangedBlock: ((CKRecord) -> Void)?

The closure to execute with the contents of a changed record.

Deprecated

var recordWithIDWasDeletedBlock: ((CKRecord.ID, CKRecord.RecordType) -> Void)?

The closure to execute when a record no longer exists.

var recordZoneChangeTokensUpdatedBlock: ((CKRecordZone.ID, CKServerChangeToken?, Data?) -> Void)?

The closure to execute when the change token updates.

var fetchRecordZoneChangesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated

