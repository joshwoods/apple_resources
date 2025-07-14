

- Network
- NWProtocolIP
- NWProtocolIP.Options
-  shouldCalculateReceiveTime 

Instance Property

# shouldCalculateReceiveTime

A Boolean that indicates whether a connection delivers receive timestamps for IP packets.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var shouldCalculateReceiveTime: Bool { get set }
```

## See Also

### Related Documentation

var receiveTime: UInt64

The time at which a packet was received, in nanoseconds, based on `CLOCK_MONOTONIC_RAW`.

### Customizing IP Behavior

var hopLimit: UInt8

The default hop limit for packets a connection generates.

var useMinimumMTU: Bool

A Boolean indicating that the connection uses the minimum MTU value, which is 1280 bytes for IPv6.

var disableFragmentation: Bool

A Boolean that indicates whether fragmentation is disabled on outbound packets.

