

- Network Extension
- NEPacketTunnelNetworkSettings
-  tunnelOverheadBytes 

Instance Property

# tunnelOverheadBytes

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var tunnelOverheadBytes: NSNumber? { get set }
```

## Discussion

The value of this property is subtracted from the Maximum Transmission Unit (MTU) of the tunnel’s underlying physical network interface to compute the MTU of the TUN interface.

## See Also

### Accessing network properties

var ipv4Settings: NEIPv4Settings?

The tunnel IP version 4 settings.

class NEIPv4Settings

The IPv4 settings of an IP layer network tunnel.

var ipv6Settings: NEIPv6Settings?

The tunnel IP version 6 settings.

class NEIPv6Settings

The IPv6 settings of an IP layer network tunnel.

var mtu: NSNumber?

The size of the maximum trasnmission unit, in bytes.

