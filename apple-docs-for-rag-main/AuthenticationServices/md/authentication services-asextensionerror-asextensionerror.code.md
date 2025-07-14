

- Authentication Services
- ASExtensionError
-  ASExtensionError.Code 

Enumeration

# ASExtensionError.Code

The codes for a credential provider extension error.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Codes

case credentialIdentityNotFound

The credential identity was not found.

case failed

The operation failed.

case userCanceled

The user canceled the operation.

case userInteractionRequired

User interaction is required.

### Enumeration Cases

case matchedExcludedCredential

This error should only be used for a passkey registration request, if the @c excludedCredentials property matches a known passkey.

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

struct ASExtensionError

A credential provider extension error.

let ASExtensionErrorDomain: String

The domain for a credential provider extension error.

