

- CloudKit
- CKError
- CKError.Code
-  CKError.Code.partialFailure 

Case

# CKError.Code.partialFailure

An error that occurs when an operation completes with partial failures.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case partialFailure
```

## Discussion

Examine the specific item failures, and act on the failed items. Each specific item error is from the CloudKit error domain. You can inspect the userInfo CKPartialErrorsByItemIDKey to see per-item errors.

Note that in a custom zone, the system processes all items in an operation atomically. As a result, you may get a CKError.Code.batchRequestFailed error for all other items in an operation that don’t cause an error.

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

