

- Core Foundation
-  CFURLError Deprecated

Enumeration

# CFURLError

`CFURL` error codes.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
enum CFURLError
```

Deprecated

Use CFError codes instead

## Topics

### Constants

case unknownError

Indicates an unknown error.

case unknownSchemeError

Indicates that the scheme is not recognized.

case resourceNotFoundError

Indicates a resource was not found.

case resourceAccessViolationError

Indicates an error in accessing a resource.

case remoteHostUnavailableError

Indicates a remote host is unavailable.

case improperArgumentsError

Indicates one or more arguments are improper.

case unknownPropertyKeyError

Indicates a property key is unknown.

case propertyKeyUnavailableError

Indicates a property key was unavailable.

case timeoutError

Indicates a timeout.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

File URL Properties

Properties for file URL resources.

HTTP URL Properties

Properties for HTTP URL resources.

