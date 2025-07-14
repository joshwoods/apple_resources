

- CloudKit
- CKError
-  CKError.Code 

Enumeration

# CKError.Code

The error codes that CloudKit returns.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
enum Code
```

## Topics

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

case missingEntitlement

An error that occurs when the app is missing a required entitlement.

case networkFailure

An error that occurs when a network is available, but CloudKit is inaccessible.

case networkUnavailable

An error that occurs when the network is unavailable.

case notAuthenticated

An error that occurs when the user is unauthenticated.

case operationCancelled

An error that occurs when an operation cancels.

case partialFailure

An error that occurs when an operation completes with partial failures.

case participantMayNeedVerification

An error that occurs when the user isn’t a participant of the share.

case permissionFailure

An error that occurs when the user doesn’t have permission to save or fetch data.

case quotaExceeded

An error that occurs when saving a record exceeds the user’s storage quota.

case referenceViolation

An error that occurs when CloudKit can’t find the target of a reference.

case requestRateLimited

An error that occurs when CloudKit rate-limits requests.

case serverRecordChanged

An error that occurs when CloudKit rejects a record because the server’s version is different.

case serverRejectedRequest

An error that occurs when CloudKit rejects the request.

case serverResponseLost

An error that occurs when CloudKit is unable to maintain the network connection and provide a response.

case serviceUnavailable

An error that occurs when CloudKit is unavailable.

case tooManyParticipants

An error that occurs when a share has too many participants.

case unknownItem

An error that occurs when the specified record doesn’t exist.

case userDeletedZone

An error that occurs when the user deletes a record zone using the Settings app.

case zoneBusy

An error that occurs when the server is too busy to handle the record zone operation.

case zoneNotFound

An error that occurs when the specified record zone doesn’t exist.

case resultsTruncated

An error that occurs when CloudKit truncates a query’s results.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

let CKErrorDomain: String

The error domain for CloudKit errors.

struct CKError

A type that describes a CloudKit error.

let CKErrorRetryAfterKey: String

The key to retrieve the number of seconds to wait before you retry a request.

let CKErrorUserDidResetEncryptedDataKey: String

The key that determines whether CloudKit deletes a record zone because of a user action.

let CKPartialErrorsByItemIDKey: String

The key to retrieve partial errors.

Record Changed Error Keys

Constants that represent conflicting records in a save operation.

