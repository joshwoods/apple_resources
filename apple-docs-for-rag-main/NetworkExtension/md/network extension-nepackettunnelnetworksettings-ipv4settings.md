

- Network Extension
- NEPacketTunnelNetworkSettings
-  ipv4Settings 

Instance Property

# ipv4Settings

The tunnel IP version 4 settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var ipv4Settings: NEIPv4Settings? { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

This property contains the IPv4 routes specifying what IPv4 traffic to route to the tunnel, as well as the IPv4 address and netmask to assign to the TUN interface.

## See Also

### Accessing network properties

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

