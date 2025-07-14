

- Network Extension
- NEFilterPacketProvider
-  packetHandler 

Instance Property

# packetHandler

A Swift closure or an ObjectiveC block that handles each packet received by the filter.

macOS 10.15+

``` source
var packetHandler: NEFilterPacketHandler? { get set }
```

## Discussion

Set this property to a handler that returns a NEFilterPacketProvider.Verdict for each packet it receives.

Since there may be multiple filtering sources presenting frames to the provider, multiple simultaneous threads may execute this packet handler. Therefore, the packet handler must be able to handle execution in a multi-threaded environment.

## See Also

### Filtering packets

typealias NEFilterPacketHandler

A type for Swift closures or ObjectiveC blocks that make filtering decisions about network packets.

class NEFilterPacketContext

The context object provided to the filter packet handler.

enum NETrafficDirection

A type to represent the direction of network traffic.

enum Verdict

The verdict returned by a packet handler indicating what the framework should do with a packet.

