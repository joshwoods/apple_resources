

- Network Extension
-  NEEthernetTunnelNetworkSettings 

Class

# NEEthernetTunnelNetworkSettings

The network settings for an ethernet-based VPN tunnel.

macOS 13.0+

``` source
class NEEthernetTunnelNetworkSettings
```

## Overview

You use this type with NEEthernetTunnelProvider instances to communicate the desired network settings for the packet tunnel to the framework. The framework takes care of applying the contained settings to the system.

Instances of this class are thread-safe.

## Topics

### Creating a settings instance

init(tunnelRemoteAddress: String, ethernetAddress: String, mtu: Int)

Creates a settings object with a given tunnel remote address and MAC address.

### Inspecting settings properties

var ethernetAddress: String

The ethernet address of the tunnel interface, as a string.

## Relationships

### Inherits From

- NEPacketTunnelNetworkSettings

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

class NEPacketTunnelNetworkSettings

The configuration for a packet tunnel provider’s virtual interface.

class NETunnelNetworkSettings

The configuration for a tunnel provider’s virtual interface.

class NEEthernetTunnelProvider

A type that implements the client side of a custom link-layer packet tunneling protocol.

