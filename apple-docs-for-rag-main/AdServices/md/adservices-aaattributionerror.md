

- AdServices
-  AAAttributionError 

Structure

# AAAttributionError

The error code that the parent class issues.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 11.1+visionOS 1.0+

``` source
struct AAAttributionError
```

## Topics

### Error domain

static var errorDomain: String

The error domain the framework uses when returning errors.

### Error codes

static var internalError: AAAttributionError.Code

The server is unable to provide a token because of an internal error.

static var networkError: AAAttributionError.Code

The server is unable to provide a token because the internet isn’t available.

static var platformNotSupported: AAAttributionError.Code

The server is unable to provide a token because of an unsupported operating system.

enum Code

The error code that the parent class issues.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let AAAttributionErrorDomain: String

The framework attribution error domain.

enum Code

The error code that the parent class issues.

