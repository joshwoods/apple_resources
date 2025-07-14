

- Network Extension
-  NEIPv6Settings 

Class

# NEIPv6Settings

The IPv6 settings of an IP layer network tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEIPv6Settings
```

## Overview

To specify the IPv6 settings of a packet tunnel, set its NEPacketTunnelNetworkSettings.ipv6Settings property to an instance of this class.

## Topics

### Initializing IPv6 settings

init(addresses: [String], networkPrefixLengths: [NSNumber])

Initializes the IPv6 settings object.

### Accessing IPv6 properties

var addresses: [String]

The IPv6 addresses to assign to the TUN interface.

var networkPrefixLengths: [NSNumber]

The IPv6 network prefix lengths to assign to the TUN interface.

### Routing network traffic

var includedRoutes: [NEIPv6Route]?

The IPv6 network traffic that the system routes to the TUN interface.

var excludedRoutes: [NEIPv6Route]?

The IPv6 network traffic that the system routes to the primary physical interface, not the TUN interface.

class NEIPv6Route

The settings for an IPv6 route.

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

### Accessing network properties

var ipv4Settings: NEIPv4Settings?

The tunnel IP version 4 settings.

class NEIPv4Settings

The IPv4 settings of an IP layer network tunnel.

var ipv6Settings: NEIPv6Settings?

The tunnel IP version 6 settings.

var tunnelOverheadBytes: NSNumber?

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

var mtu: NSNumber?

The size of the maximum trasnmission unit, in bytes.

