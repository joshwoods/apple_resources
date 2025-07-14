

- Network Extension
-  NEDNSProxyManagerError 

Enumeration

# NEDNSProxyManagerError

The possible DNS proxy manager errors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum NEDNSProxyManagerError
```

## Overview

These errors appear as the parameter in the completion handler of the methods that you use to manage DNS proxy configuration: loadFromPreferences(completionHandler:), removeFromPreferences(completionHandler:), and saveToPreferences(completionHandler:).

## Topics

### Enumeration Cases

case configurationInvalid

Invalid DNS proxy configuration that cannot be stored.

case configurationDisabled

Disabled DNS proxy configuration.

case configurationStale

Outdated DNS proxy configuration that needs to be loaded.

case configurationCannotBeRemoved

Unremovable DNS proxy configuration.

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

let NEDNSProxyErrorDomain: String

The DNS proxy error domain.

