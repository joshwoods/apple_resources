

- CloudKit
- CKError
- CKError.Code
-  CKError.Code.accountTemporarilyUnavailable 

Case

# CKError.Code.accountTemporarilyUnavailable

An error that occurs when the user’s iCloud account is temporarily unavailable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case accountTemporarilyUnavailable
```

## Discussion

You receive this error when the user’s iCloud account is available, but isn’t ready to support CloudKit operations. Don’t delete any cached data and don’t enqueue any additional CloudKit operations.

Checking the account status after the operation fails, assuming there are no other changes to the account’s status, returns CKAccountStatus.temporarilyUnavailable. Use the CKAccountChanged notification to listen for future account status changes, and retry the operation after the status becomes CKAccountStatus.available.

## See Also

### Error Codes

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

case missingEntitlement

An error that occurs when the app is missing a required entitlement.

