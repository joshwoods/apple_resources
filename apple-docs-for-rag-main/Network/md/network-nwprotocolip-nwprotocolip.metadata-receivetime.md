

- Network
- NWProtocolIP
- NWProtocolIP.Metadata
-  receiveTime 

Instance Property

# receiveTime

The time at which a packet was received, in nanoseconds, based on `CLOCK_MONOTONIC_RAW`.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var receiveTime: UInt64 { get }
```

## See Also

### Related Documentation

var shouldCalculateReceiveTime: Bool

A Boolean that indicates whether a connection delivers receive timestamps for IP packets.

