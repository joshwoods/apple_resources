

- Network Extension
-  NEFilterManagerError 

Enumeration

# NEFilterManagerError

Error codes specific to filter managers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
enum NEFilterManagerError
```

## Topics

### Error codes

case configurationInvalid

An error code that indicates the filter configuration is invalid.

case configurationDisabled

An error code that indicates the filter configuration isn’t enabled.

case configurationStale

An error code that indicates another process modfied the filter configuration since the last time the app loaded the configuration.

case configurationCannotBeRemoved

An error code that indicates removing the configuration isn’t allowed.

case configurationPermissionDenied

An error code that indicates the configuration lacks permission.

case configurationInternalError

An error code that indicates an internal configuration error occurred.

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

### Errors

let NEFilterErrorDomain: String

The domain for errors resulting from calls to the filter manager.

