

- Network Extension
-  NEDNSSettingsManagerError 

Enumeration

# NEDNSSettingsManagerError

Error codes specific to DNS managers.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum NEDNSSettingsManagerError
```

## Topics

### Error codes

case configurationInvalid

An error code that indicates the DNS settings manager is invalid.

case configurationDisabled

An error code that indicates the DNS settings manager isn’t enabled.

case configurationStale

An error code that indicates the DNS settings manager isn’t loaded.

case configurationCannotBeRemoved

An error code that indicates removing the DNS settings manager failed.

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

let NEDNSSettingsErrorDomain: String

The domain for errors resulting from calls to the DNS settings manager.

