

- Network Extension
-  NETunnelNetworkSettings 

Class

# NETunnelNetworkSettings

The configuration for a tunnel provider’s virtual interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NETunnelNetworkSettings
```

## Topics

### Initializing tunnel network settings

init(tunnelRemoteAddress: String)

Initialize a `NETunnelNetworkSettings` object.

### Accessing tunnel network settings

var tunnelRemoteAddress: String

The IP address of the tunnel server.

var dnsSettings: NEDNSSettings?

The tunnel DNS settings.

class NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

var proxySettings: NEProxySettings?

The tunnel HTTP proxy settings.

class NEProxySettings

`NEProxySettings` contains HTTP proxy settings.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEPacketTunnelNetworkSettings
- NETransparentProxyNetworkSettings

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

### App proxy provider

class NEAppProxyProvider

The principal class for an app proxy provider app extension.

class NETunnelProvider

An abstract base class shared by NEPacketTunnelProvider and NEAppProxyProvider.

class NEProvider

An abstract base class for all NetworkExtension providers.

