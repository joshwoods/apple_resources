

- Network Extension
- NEPacketTunnelNetworkSettings
-  mtu 

Instance Property

# mtu

The size of the maximum trasnmission unit, in bytes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var mtu: NSNumber? { get set }
```

## Discussion

The maximum transmission unit (MTU) size represents the largest number of bytes that anything can assign to the TUN interface.

Note

The system ignores the tunnelOverheadBytes property when this property is non-`nil`.

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

var tunnelOverheadBytes: NSNumber?

The number of bytes added to each tunneled packet for storing tunneling protocol headers.

