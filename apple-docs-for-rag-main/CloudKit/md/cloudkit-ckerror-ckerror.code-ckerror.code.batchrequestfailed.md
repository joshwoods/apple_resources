

- CloudKit
- CKError
- CKError.Code
-  CKError.Code.batchRequestFailed 

Case

# CKError.Code.batchRequestFailed

An error that occurs when the system rejects the entire batch of changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
case batchRequestFailed
```

## Discussion

This error occurs when an operation attempts to save multiple items in a custom zone, but one of those items encounters an error. Because custom zones are atomic, the entire batch fails. The items that cause the problem have their own errors, and all other items in the batch have a CKError.Code.batchRequestFailed error to indicate that the system can’t save them.

This error indicates that the system can’t process the associated item due to an error in another item in the operation. Check the other per-item errors under CKPartialErrorsByItemIDKey for any that aren’t CKError.Code.batchRequestFailed errors. Handle those errors, and then retry all items in the operation.

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

