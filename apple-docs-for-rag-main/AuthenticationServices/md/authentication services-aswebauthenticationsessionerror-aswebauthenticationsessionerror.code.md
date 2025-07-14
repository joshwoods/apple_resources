

- Authentication Services
- ASWebAuthenticationSessionError
-  ASWebAuthenticationSessionError.Code 

Enumeration

# ASWebAuthenticationSessionError.Code

The error code for a web authentication session error.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.15+tvOS 16.0+visionOS 1.0+watchOS 6.2+

``` source
enum Code
```

## Topics

### Codes

case canceledLogin

The login has been canceled.

case presentationContextNotProvided

A context wasn’t provided.

case presentationContextInvalid

The context was invalid.

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

### Recognizing Errors

struct ASWebAuthenticationSessionError

Errors that a web authentication session can generate.

let ASWebAuthenticationSessionErrorDomain: String

The error domain for a web authentication session.

