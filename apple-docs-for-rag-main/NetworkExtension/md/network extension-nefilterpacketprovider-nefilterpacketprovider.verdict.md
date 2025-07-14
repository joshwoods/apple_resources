

- Network Extension
- NEFilterPacketProvider
-  NEFilterPacketProvider.Verdict 

Enumeration

# NEFilterPacketProvider.Verdict

The verdict returned by a packet handler indicating what the framework should do with a packet.

macOS 10.15+

``` source
enum Verdict
```

## Topics

### Verdicts

case allow

A verdict to allow a packet.

case drop

A verdict to drop a packet.

case delay

A verdict to delay a packet until a future verdict.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Filtering packets

var packetHandler: NEFilterPacketHandler?

A Swift closure or an ObjectiveC block that handles each packet received by the filter.

typealias NEFilterPacketHandler

A type for Swift closures or ObjectiveC blocks that make filtering decisions about network packets.

class NEFilterPacketContext

The context object provided to the filter packet handler.

enum NETrafficDirection

A type to represent the direction of network traffic.

