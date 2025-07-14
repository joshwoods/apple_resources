

- Network
- NWConnection
- NWConnection.DataTransferReport
- NWConnection.DataTransferReport.PathReport
-  retransmittedTransportByteCount 

Instance Property

# retransmittedTransportByteCount

The number of bytes the transport protocol retransmitted.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let retransmittedTransportByteCount: UInt64
```

## See Also

### Inspecting Transport Metrics

let receivedTransportByteCount: UInt64

The number of bytes the transport protocol delivered.

let receivedTransportDuplicateByteCount: UInt64

The number of duplicated bytes the transport protocol detected.

let receivedTransportOutOfOrderByteCount: UInt64

The number of bytes the transport protocol received out of order.

let sentTransportByteCount: UInt64

The number of bytes sent into the transport protocol.

let transportSmoothedRTT: TimeInterval

The smoothed round-trip time the transport protocol measured.

let transportMinimumRTT: TimeInterval

The minimum round-trip time the transport protocol measured.

let transportRTTVariance: TimeInterval

The variance of the round-trip time the transport protocol measured.

