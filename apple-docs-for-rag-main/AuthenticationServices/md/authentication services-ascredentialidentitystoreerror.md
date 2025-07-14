

- Authentication Services
-  ASCredentialIdentityStoreError 

Structure

# ASCredentialIdentityStoreError

A credential identity store error.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct ASCredentialIdentityStoreError
```

## Topics

### Error domain

let ASCredentialIdentityStoreErrorDomain: String

The domain for a credential identity store error.

static var internalError: ASCredentialIdentityStoreError.Code

The operation failed due to an internal error.

static var storeBusy: ASCredentialIdentityStoreError.Code

The operation failed because the credential identity store is busy.

static var storeDisabled: ASCredentialIdentityStoreError.Code

The operation failed because the credential identity store is disabled.

enum Code

Constants that represent credential identity store error codes.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Recognizing errors

let ASCredentialIdentityStoreErrorDomain: String

The domain for a credential identity store error.

enum Code

Constants that represent credential identity store error codes.

