

- Network Extension
-  NEIPv4Settings 

Class

# NEIPv4Settings

The IPv4 settings of an IP layer network tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEIPv4Settings
```

## Overview

To specify the IPv4 settings of a packet tunnel, set its NEPacketTunnelNetworkSettings.ipv4Settings property to an instance of this class.

## Topics

### Initializing IPv4 settings

init(addresses: [String], subnetMasks: [String])

Initializes an IPv4 settings object.

### Accessing IPv4 properties

var addresses: [String]

The IPv4 addresses to assign to the TUN interface.

var subnetMasks: [String]

The IPv4 network masks to assign to the TUN interface.

var router: String?

The address of the next-hop gateway router represented as a dotted decimal string.

### Routing network traffic

var includedRoutes: [NEIPv4Route]?

The IPv4 network traffic that the system routes to the TUN interface.

var excludedRoutes: [NEIPv4Route]?

The IPv4 network traffic that the system routes to the primary physical interface, not the TUN interface.

class NEIPv4Route

The settings for an IPv4 route.

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

var ipv6Settings: NEIPv6Settings?

The tunnel IP version 6 settings.

class NEIPv6Settings

The IPv6 settings of an IP layer network tunnel.

var tunnelOverheadBytes: NSNumber?

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

var mtu: NSNumber?

The size of the maximum trasnmission unit, in bytes.

