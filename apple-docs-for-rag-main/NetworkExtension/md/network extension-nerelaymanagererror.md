

- Network Extension
-  NERelayManagerError 

Enumeration

# NERelayManagerError

Error codes specific to relay managers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum NERelayManagerError
```

## Topics

### Error codes

case configurationInvalid

An error code that indicates the relay manager is invalid.

case configurationDisabled

An error code that indicates the relay manager isn’t enabled.

case configurationStale

An error code that indicates the relay manager isn’t loaded.

case configurationCannotBeRemoved

An error code that indicates removing the relay manager failed.

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

let NERelayErrorDomain: String

The domain for errors resulting from calls to the relay manager.

