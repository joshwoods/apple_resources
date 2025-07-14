

- AdServices
- AAAttributionError
-  AAAttributionError.Code 

Enumeration

# AAAttributionError.Code

The error code that the parent class issues.

iOS 14.3+iPadOS 14.3+Mac Catalyst 14.3+macOS 11.1+visionOS 1.0+

``` source
enum Code
```

## Topics

### Creating an error code

init?(rawValue: Int)

Creates an error code structure with the specified raw value.

### Determining the cause of an error

case internalError

The server is unable to provide a token because of an internal error.

case networkError

The server is unable to provide a token because the internet isn’t available.

case platformNotSupported

The server is unable to provide a token because of an unsupported operating system.

### Getting information about error codes

var localizedDescription: String { get }

Retrieve the localized description for this error.

### Comparing errors

func != (lhs: (), rhs: ()) -> Bool

Returns a Boolean value indicating whether any corresponding components of the two tuples are not equal.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct AAAttributionError

The error code that the parent class issues.

let AAAttributionErrorDomain: String

The framework attribution error domain.

