

- Authentication Services
- ASCredentialIdentityStoreError
-  ASCredentialIdentityStoreError.Code 

Enumeration

# ASCredentialIdentityStoreError.Code

Constants that represent credential identity store error codes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Codes

case internalError

The operation failed due to an internal error.

case storeBusy

The operation failed because the credential identity store is busy.

case storeDisabled

The operation failed because the credential identity store is disabled.

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

### Recognizing errors

struct ASCredentialIdentityStoreError

A credential identity store error.

let ASCredentialIdentityStoreErrorDomain: String

The domain for a credential identity store error.

