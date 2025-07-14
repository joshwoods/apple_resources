

- Network Extension
- NEAppPushManagerError
-  NEAppPushManagerError.Code 

Enumeration

# NEAppPushManagerError.Code

Error codes that the local push API declares.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error codes

case configurationInvalid

An error code that indicates the app push configuration is invalid.

case configurationNotLoaded

An error code that indicates the manager hasn’t loaded the app push configuration.

case inactiveSession

An error code that indicates an invalid attempt to perform an operation on an inactive session.

case internalError

An error code that indicates an internal error in the local push connectivity framework.

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

### Handling errors

struct NEAppPushManagerError

An error that the push manager encounters.

let NEAppPushErrorDomain: String

The error domain string for local push errors.

