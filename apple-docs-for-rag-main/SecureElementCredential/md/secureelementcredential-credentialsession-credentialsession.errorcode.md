

- SecureElementCredential
- CredentialSession
-  CredentialSession.ErrorCode 

Enumeration

# CredentialSession.ErrorCode

An error encountered by a credential session.

iOS 18.1+iPadOS 18.1+

``` source
enum ErrorCode
```

## Topics

### Authorization and permission error codes

case userNotAuthorized

The person using the app isn’t authorized to perform the operation.

case accessDenied

The person using the app declined to grant permission for the operation.

case clientNotInForeground

Your app isn’t in the foreground, which is required to use the credential session.

case userCanceledAuthorization

The person using the app dismissed the authorization sheet.

case userAuthorizationTimedOut

Authorization timed out while waiting for the person using the app.

case featureUnavailable

The feature is unavailable.

case ineligible

The current device and user configuation are ineligible to use this service.

case conditionsNotSatisfied

The iCloud account or passcode of the person using the app don’t satisfy the conditions to use this service.

### Credential error codes

case invalidCredentialState

A credential is in a state that doesn’t permit that function.

case credentialDoesNotExist

The credential doesn’t exist, or you don’t have access to it.

case instanceDoesNotExist

The instance doesn’t exist in the target credential.

### Session error codes

case invalidSessionState

The session is in a state that doesn’t permit that function.

case sessionInvalidated

The client requested invalidation of the session.

### Command error codes

case commandNotSupported

Your app attempted an unsupported Secure Element command.

### Network-related error codes

case network

The device’s internet connection is offline.

### Presentment intent assertion error codes

case presentmentIntentAssertionTimeout

The presentment intent assertion timed out.

### UIKit error codes

case invalidView

The provided UIKit view is invalid.

### Hardware error codes

case insufficientSpace

The hardware storage has insufficient space for the attempted provisioning.

### Temporary error codes

case resourceUnavailable

The requested resource is unavailable.

case acquiredResourceRelinquished

The system relinquished an underlying shared resource, preventing the operation from completing.

### Miscellaneous error codes

case invalidInput

One or more parameters is invalid.

case internalError

The framework encountered an internal error.

### Inspecting error causes

var failureReason: String?

A human-readable description of the error reason.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Comparing error codes

static func == (CredentialSession.ErrorCode, CredentialSession.ErrorCode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

