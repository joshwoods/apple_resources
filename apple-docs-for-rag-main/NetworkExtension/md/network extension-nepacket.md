

- Network Extension
-  NEPacket 

Class

# NEPacket

A network packet and its associated properties.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 17.0+visionOS 1.0+

``` source
class NEPacket
```

## Topics

### Initializing a packet

init(data: Data, protocolFamily: sa_family_t)

### Accessing packet properties

var data: Data

var metadata: NEFlowMetaData?

var protocolFamily: sa_family_t

var direction: NETrafficDirection

The direction of the packet.

enum NETrafficDirection

A type to represent the direction of network traffic.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Packet handling

class NEPacketTunnelFlow

An object you use to read and write packets to and from the tunnel’s virtual interface.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

