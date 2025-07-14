

- CloudKit
- CKError
-  accountTemporarilyUnavailable 

Type Property

# accountTemporarilyUnavailable

An error that occurs when the user’s iCloud account is temporarily unavailable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var accountTemporarilyUnavailable: CKError.Code { get }
```

## Discussion

You receive this error when the user’s iCloud account is available, but isn’t ready to support CloudKit operations. Don’t delete any cached data and don’t enqueue any additional CloudKit operations.

Checking the account status after the operation fails, assuming there are no other changes to the account’s status, returns CKAccountStatus.temporarilyUnavailable. Use the CKAccountChanged notification to listen for future account status changes, and retry the operation after the status becomes CKAccountStatus.available.

## See Also

### Getting Error Codes

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

static var missingEntitlement: CKError.Code

An error that occurs when the app is missing a required entitlement.

