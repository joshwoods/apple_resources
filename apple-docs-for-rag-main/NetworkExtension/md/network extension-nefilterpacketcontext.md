

- Network Extension
-  NEFilterPacketContext 

Class

# NEFilterPacketContext

The context object provided to the filter packet handler.

macOS 10.15+

``` source
class NEFilterPacketContext
```

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Filtering packets

var packetHandler: NEFilterPacketHandler?

A Swift closure or an ObjectiveC block that handles each packet received by the filter.

typealias NEFilterPacketHandler

A type for Swift closures or ObjectiveC blocks that make filtering decisions about network packets.

enum NETrafficDirection

A type to represent the direction of network traffic.

enum Verdict

The verdict returned by a packet handler indicating what the framework should do with a packet.

