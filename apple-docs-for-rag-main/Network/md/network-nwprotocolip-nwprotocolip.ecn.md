

- Network
- NWProtocolIP
-  NWProtocolIP.ECN 

Enumeration

# NWProtocolIP.ECN

Flag values for Explicit Congestion Notifications in IP packets.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum ECN
```

## Topics

### ECN Flags

case nonECT

Non-ECN Capable Transport.

case ect0

ECN Capable Transport (flag 0).

case ect1

ECN Capable Transport (flag 1).

case ce

Congestion Experienced.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Sending IP Options

init()

Initializes an IP packet configuration with default settings.

var ecn: NWProtocolIP.ECN

A specific Explicit Congestion Notification flag value to set on an IP packet.

var serviceClass: NWParameters.ServiceClass

A specific service class to mark on an IP packet.

