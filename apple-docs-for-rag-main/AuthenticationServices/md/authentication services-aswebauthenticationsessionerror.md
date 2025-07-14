

- Authentication Services
-  ASWebAuthenticationSessionError 

Structure

# ASWebAuthenticationSessionError

Errors that a web authentication session can generate.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.15+tvOS 16.0+visionOS 1.0+watchOS 6.2+

``` source
struct ASWebAuthenticationSessionError
```

## Topics

### Error Domain

let ASWebAuthenticationSessionErrorDomain: String

The error domain for a web authentication session.

### Error Codes

static var canceledLogin: ASWebAuthenticationSessionError.Code

The login has been canceled.

static var presentationContextNotProvided: ASWebAuthenticationSessionError.Code

A context wasn’t provided.

static var presentationContextInvalid: ASWebAuthenticationSessionError.Code

The context was invalid.

enum Code

The error code for a web authentication session error.

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

### Recognizing Errors

let ASWebAuthenticationSessionErrorDomain: String

The error domain for a web authentication session.

enum Code

The error code for a web authentication session error.

