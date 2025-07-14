

- CloudKit
- CKFetchDatabaseChangesOperation
-  fetchDatabaseChangesCompletionBlock Deprecated

Instance Property

# fetchDatabaseChangesCompletionBlock

The closure to execute when the operation finishes.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedtvOS 10.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var fetchDatabaseChangesCompletionBlock: ((CKServerChangeToken?, Bool, (any Error)?) -> Void)? { get set }
```

Deprecated

Use fetchDatabaseChangesResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- The change token to store and use in subsequent instances of CKFetchDatabaseChangesOperation.

- A Boolen value that indicates whether this is the final database change. If fetchAllChanges is false, it’s the app’s responsibility to create additional instances of CKFetchDatabaseChangesOperation to fetch further changes.

- An error object that contains information about a problem, or `nil` if CloudKit successfully retrieves the database changes.

Note

The change token and error parameters are mutally exclusive — that is, the closure provides one of them but not both.

Your app is responsible for saving the change token at the end of the operation and providing it to future uses of CKFetchDatabaseChangesOperation. If the server returns a CKError.Code.changeTokenExpired error, the previousServerChangeToken value is stale and your app needs to clear its local cache and refetch the database changes, starting with a `nil` change token.

## See Also

### Processing the Operation’s Results

var recordZoneWithIDChangedBlock: ((CKRecordZone.ID) -> Void)?

The closure to execute with a single record zone change.

var recordZoneWithIDWasDeletedBlock: ((CKRecordZone.ID) -> Void)?

The closure to execute when a record zone no longer exists.

var recordZoneWithIDWasDeletedDueToUserEncryptedDataResetBlock: ((CKRecordZone.ID) -> Void)?

The closure to execute when a user-invoked account reset deletes a record zone.

var recordZoneWithIDWasPurgedBlock: ((CKRecordZone.ID) -> Void)?

The closure to execute when CloudKit purges a record zone.

var changeTokenUpdatedBlock: ((CKServerChangeToken) -> Void)?

The closure to execute when the change token updates.

