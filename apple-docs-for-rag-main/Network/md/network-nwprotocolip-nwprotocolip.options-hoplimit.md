

- Network
- NWProtocolIP
- NWProtocolIP.Options
-  hopLimit 

Instance Property

# hopLimit

The default hop limit for packets a connection generates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var hopLimit: UInt8 { get set }
```

## See Also

### Customizing IP Behavior

var shouldCalculateReceiveTime: Bool

A Boolean that indicates whether a connection delivers receive timestamps for IP packets.

var useMinimumMTU: Bool

A Boolean indicating that the connection uses the minimum MTU value, which is 1280 bytes for IPv6.

var disableFragmentation: Bool

A Boolean that indicates whether fragmentation is disabled on outbound packets.

