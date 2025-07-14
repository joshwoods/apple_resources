

- Network
- NWProtocolIP
-  NWProtocolIP.Metadata 

Class

# NWProtocolIP.Metadata

Per-packet IP metadata you configure when sending and receiving packets.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class Metadata
```

## Topics

### Sending IP Options

init()

Initializes an IP packet configuration with default settings.

var ecn: NWProtocolIP.ECN

A specific Explicit Congestion Notification flag value to set on an IP packet.

enum ECN

Flag values for Explicit Congestion Notifications in IP packets.

var serviceClass: NWParameters.ServiceClass

A specific service class to mark on an IP packet.

### Receiving IP Packets

var receiveTime: UInt64

The time at which a packet was received, in nanoseconds, based on `CLOCK_MONOTONIC_RAW`.

## Relationships

### Inherits From

- NWProtocolMetadata

### Conforms To

- Sendable

