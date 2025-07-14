

- Authentication Services
-  ASExtensionError 

Structure

# ASExtensionError

A credential provider extension error.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
struct ASExtensionError
```

## Topics

### Identifying the error domain

let ASExtensionErrorDomain: String

The domain for a credential provider extension error.

### Error codes

static var credentialIdentityNotFound: ASExtensionError.Code

The credential identity was not found.

static var failed: ASExtensionError.Code

The operation failed.

static var userCanceled: ASExtensionError.Code

The user canceled the operation.

static var userInteractionRequired: ASExtensionError.Code

User interaction is required.

enum Code

The codes for a credential provider extension error.

### Type Properties

static var errorDomain: String

static var matchedExcludedCredential: ASExtensionError.Code

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Recognizing errors

let ASExtensionErrorDomain: String

The domain for a credential provider extension error.

enum Code

The codes for a credential provider extension error.

