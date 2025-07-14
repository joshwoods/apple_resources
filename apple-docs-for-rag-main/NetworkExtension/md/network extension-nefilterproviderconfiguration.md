

- Network Extension
-  NEFilterProviderConfiguration 

Class

# NEFilterProviderConfiguration

Configuration parameters for a content filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEFilterProviderConfiguration
```

## Topics

### Configuring filter behavior

var filterBrowsers: Bool

A Boolean value that indicates that the system applies the filter to flows of network data originated from WebKit browser objects.

var filterSockets: Bool

A Boolean value that indicates that the system applies the filter to flows of network data originated from sockets.

var filterPackets: Bool

A Boolean value that indicates that the system applies the filter to packets of network data.

### Accessing the filter configuration

var vendorConfiguration: [String : Any]?

A dictionary of provider-specific configuration settings.

var serverAddress: String?

The address of a server that the Filter Control Provider may contact for rules and other configuration information.

var username: String?

A string that identifies the user.

var organization: String?

A string that identifies the organization that administers the filter.

var passwordReference: Data?

A persistent reference to a keychain item containing a password associated with the filter.

var identityReference: Data?

A persistent reference to a keychain item containing a certificate and private key associated with the filter.

### Accessing bundle identifiers

var filterDataProviderBundleIdentifier: String?

The bundle identifier of the filter data provider system extension.

var filterPacketProviderBundleIdentifier: String?

The bundle identifier of the filter packet provider system extension.

## Relationships

### Inherits From

- NSObject

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

### Filter configuration

class NEFilterManager

An object to create and manage a content filter’s configuration.

