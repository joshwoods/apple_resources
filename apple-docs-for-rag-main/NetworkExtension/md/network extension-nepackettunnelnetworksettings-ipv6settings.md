

- Network Extension
- NEPacketTunnelNetworkSettings
-  ipv6Settings 

Instance Property

# ipv6Settings

The tunnel IP version 6 settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var ipv6Settings: NEIPv6Settings? { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

This property contains the IPv6 routes specifying what IPv6 traffic to route to the tunnel, as well as the IPv6 address and network prefix to assign to the TUN interface.

## See Also

### Accessing network properties

var ipv4Settings: NEIPv4Settings?

The tunnel IP version 4 settings.

class NEIPv4Settings

The IPv4 settings of an IP layer network tunnel.

class NEIPv6Settings

The IPv6 settings of an IP layer network tunnel.

var tunnelOverheadBytes: NSNumber?

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

var mtu: NSNumber?

The size of the maximum trasnmission unit, in bytes.

