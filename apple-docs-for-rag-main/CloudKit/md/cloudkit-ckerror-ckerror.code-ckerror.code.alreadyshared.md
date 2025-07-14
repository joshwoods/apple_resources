

- CloudKit
- CKError
- CKError.Code
-  CKError.Code.alreadyShared 

Case

# CKError.Code.alreadyShared

An error that occurs when CloudKit attempts to share a record with an existing share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case alreadyShared
```

## Discussion

A record can exist in only a single share at a time. This error means that one of the following conditions exists:

- The record already has an existing share.

- The record has a parent, and its parent has a share.

- The record is a parent, and one of its children has a share.

## See Also

### Error Codes

case accountTemporarilyUnavailable

An error that occurs when the user’s iCloud account is temporarily unavailable.

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

