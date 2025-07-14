

- CloudKit
- CKError
-  referenceViolation 

Type Property

# referenceViolation

An error that occurs when CloudKit can’t find the target of a reference.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static var referenceViolation: CKError.Code { get }
```

## See Also

### Getting Error Codes

static var accountTemporarilyUnavailable: CKError.Code

An error that occurs when the user’s iCloud account is temporarily unavailable.

static var alreadyShared: CKError.Code

An error that occurs when CloudKit attempts to share a record with an existing share.

static var assetFileModified: CKError.Code

An error that occurs when the system modifies an asset while saving it.

static var assetFileNotFound: CKError.Code

An error that occurs when the system can’t find the specified asset.

static var assetNotAvailable: CKError.Code

An error that occurs when the system can’t access the specified asset.

static var badContainer: CKError.Code

An error that occurs when you use an unknown or unauthorized container.

static var badDatabase: CKError.Code

An error that occurs when the operation can’t complete for the specified database.

static var batchRequestFailed: CKError.Code

An error that occurs when the system rejects the entire batch of changes.

static var changeTokenExpired: CKError.Code

An error that occurs when the change token expires.

static var constraintViolation: CKError.Code

An error that occurs when the server rejects the request because of a unique constraint violation.

static var incompatibleVersion: CKError.Code

An error that occurs when the current app version is older than the oldest allowed version.

static var internalError: CKError.Code

A nonrecoverable error that CloudKit encounters.

static var invalidArguments: CKError.Code

An error that occurs when the request contains invalid information.

static var limitExceeded: CKError.Code

An error that occurs when a request’s size exceeds the limit.

static var managedAccountRestricted: CKError.Code

An error that occurs when CloudKit rejects a request due to a managed-account restriction.

