

- Network Extension
-  NEFilterPacketProvider 

Class

# NEFilterPacketProvider

A filter provider that evaluates network packets and decides whether to block, allow, or delay the packets.

macOS 10.15+

``` source
class NEFilterPacketProvider
```

## Topics

### Filtering packets

var packetHandler: NEFilterPacketHandler?

A Swift closure or an ObjectiveC block that handles each packet received by the filter.

typealias NEFilterPacketHandler

A type for Swift closures or ObjectiveC blocks that make filtering decisions about network packets.

class NEFilterPacketContext

The context object provided to the filter packet handler.

enum NETrafficDirection

A type to represent the direction of network traffic.

enum Verdict

The verdict returned by a packet handler indicating what the framework should do with a packet.

### Delaying packets

func delayCurrentPacket(NEFilterPacketContext) -> NEPacket

Delay a packet currently processed by a packet handler.

func allow(NEPacket)

Allow delivery of a previously-delayed packet.

### Instance Properties

var handler: ((NEFilterPacketContext, NWInterface, NETrafficDirection, UnsafeRawBufferPointer) -> NEFilterPacketProvider.Verdict)?

## Relationships

### Inherits From

- NEFilterProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Data and control providers

class NEFilterDataProvider

The principal class for a filter data provider extension.

class NEFilterControlProvider

The principal class for a filter control provider extension.

class NEFilterProvider

An abstract base class shared by content filters.

