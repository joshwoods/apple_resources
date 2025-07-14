

- CloudKit
- CKError
- CKError.Code
-  CKError.Code.serverRecordChanged 

Case

# CKError.Code.serverRecordChanged

An error that occurs when CloudKit rejects a record because the server’s version is different.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case serverRecordChanged
```

## Discussion

This error indicates that the server’s version of the record is newer than the local version the client’s trying to save. Your app needs to handle this error, resolve any conflicts in the record, and attempt another save of the record, if necessary.

CloudKit provides your app with three copies of the record in this error’s `userInfo` dictionary to assist with comparing and merging the changes:

- CKRecordChangedErrorClientRecordKey: The local record that the client’s trying to save.

- CKRecordChangedErrorServerRecordKey: The record that exists on the server.

- CKRecordChangedErrorAncestorRecordKey: The original version of the record.

When a conflict occurs, your app needs to merge all changes into the record for the CKRecordChangedErrorServerRecordKey key and attempt a new save using that record. Merging into either of the other two copies of the record results in another conflict error because those records have the old record change tag.

## See Also

### Error Codes

case accountTemporarilyUnavailable

An error that occurs when the user’s iCloud account is temporarily unavailable.

case alreadyShared

An error that occurs when CloudKit attempts to share a record with an existing share.

case assetFileModified

An error that occurs when the system modifies an asset while saving it.

case assetFileNotFound

An error that occurs when the system can’t find the specified asset.

case assetNotAvailable

An error that occurs when the system can’t access the specified asset.

case badContainer

An error that occurs when you use an unknown or unauthorized container.

case badDatabase

An error that occurs when the operation can’t complete for the specified database.

case batchRequestFailed

An error that occurs when the system rejects the entire batch of changes.

case changeTokenExpired

An error that occurs when the change token expires.

case constraintViolation

An error that occurs when the server rejects the request because of a unique constraint violation.

case incompatibleVersion

An error that occurs when the current app version is older than the oldest allowed version.

case internalError

A nonrecoverable error that CloudKit encounters.

case invalidArguments

An error that occurs when the request contains invalid information.

case limitExceeded

An error that occurs when a request’s size exceeds the limit.

case managedAccountRestricted

An error that occurs when CloudKit rejects a request due to a managed-account restriction.

