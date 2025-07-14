

- Network
- NWConnection
- NWConnection.DataTransferReport
-  NWConnection.DataTransferReport.PathReport 

Structure

# NWConnection.DataTransferReport.PathReport

A report that contains details about data transfer over a single network path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct PathReport
```

## Topics

### Identifying Paths

let interface: NWInterface

The network interface this path used.

### Inspecting Application Metrics

let receivedApplicationByteCount: UInt64

The number of bytes the connection delivered.

let sentApplicationByteCount: UInt64

The number of bytes sent on the connection.

### Inspecting Transport Metrics

let receivedTransportByteCount: UInt64

The number of bytes the transport protocol delivered.

let receivedTransportDuplicateByteCount: UInt64

The number of duplicated bytes the transport protocol detected.

let receivedTransportOutOfOrderByteCount: UInt64

The number of bytes the transport protocol received out of order.

let sentTransportByteCount: UInt64

The number of bytes sent into the transport protocol.

let retransmittedTransportByteCount: UInt64

The number of bytes the transport protocol retransmitted.

let transportSmoothedRTT: TimeInterval

The smoothed round-trip time the transport protocol measured.

let transportMinimumRTT: TimeInterval

The minimum round-trip time the transport protocol measured.

let transportRTTVariance: TimeInterval

The variance of the round-trip time the transport protocol measured.

### Inspecting Packet Metrics

let receivedIPPacketCount: UInt64

The number of IP packets the connection received.

let sentIPPacketCount: UInt64

The number of IP packets the connection sent.

### Instance Properties

var radioType: NWInterface.RadioType?

## Relationships

### Conforms To

- Sendable

## See Also

### Examining Data Transfer

let aggregatePathReport: NWConnection.DataTransferReport.PathReport

A report that sums counts across all network paths.

let pathReports: [NWConnection.DataTransferReport.PathReport]

An array of reports for each network path the connection used.

