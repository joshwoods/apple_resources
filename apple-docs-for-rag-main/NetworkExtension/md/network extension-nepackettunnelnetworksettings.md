

- Network Extension
-  NEPacketTunnelNetworkSettings 

Class

# NEPacketTunnelNetworkSettings

The configuration for a packet tunnel provider’s virtual interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEPacketTunnelNetworkSettings
```

## Mentioned in 

Routing your VPN network traffic

## Topics

### Accessing network properties

var ipv4Settings: NEIPv4Settings?

The tunnel IP version 4 settings.

class NEIPv4Settings

The IPv4 settings of an IP layer network tunnel.

var ipv6Settings: NEIPv6Settings?

The tunnel IP version 6 settings.

class NEIPv6Settings

The IPv6 settings of an IP layer network tunnel.

var tunnelOverheadBytes: NSNumber?

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

var mtu: NSNumber?

The size of the maximum trasnmission unit, in bytes.

## Relationships

### Inherits From

- NETunnelNetworkSettings

### Inherited By

- NEEthernetTunnelNetworkSettings

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

### Packet tunnel provider

class NEPacketTunnelProvider

The principal class for a packet tunnel provider app extension.

class NETunnelProvider

An abstract base class shared by NEPacketTunnelProvider and NEAppProxyProvider.

class NEProvider

An abstract base class for all NetworkExtension providers.

class NETunnelNetworkSettings

The configuration for a tunnel provider’s virtual interface.

class NEEthernetTunnelProvider

A type that implements the client side of a custom link-layer packet tunneling protocol.

class NEEthernetTunnelNetworkSettings

The network settings for an ethernet-based VPN tunnel.

