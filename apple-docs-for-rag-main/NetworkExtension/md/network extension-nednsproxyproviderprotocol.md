

- Network Extension
-  NEDNSProxyProviderProtocol 

Class

# NEDNSProxyProviderProtocol

Configuration parameters for a DNS proxy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
class NEDNSProxyProviderProtocol
```

## Topics

### Accessing the DNS proxy configuration

var providerConfiguration: [String : Any]?

A dictionary containing vendor-specific configuration parameters for a proxy provider.

var providerBundleIdentifier: String?

A string containing the bundle identifier of the proxy provider to be used by this configuration.

## Relationships

### Inherits From

- NEVPNProtocol

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Configuration

class NEDNSProxyManager

An object to create and manage an DNS proxy provider’s configuration.

