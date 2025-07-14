

- Network Extension
-  NEFilterPacketHandler 

Type Alias

# NEFilterPacketHandler

A type for Swift closures or ObjectiveC blocks that make filtering decisions about network packets.

macOS 10.15+

``` source
typealias NEFilterPacketHandler = (NEFilterPacketContext, nw_interface_t, NETrafficDirection, UnsafeRawPointer, Int) -> NEFilterPacketProvider.Verdict
```

## Parameters 

`context`  

The current filtering context.

`interface`  

The ingress or egress interface of the packet.

`direction`  

The direction the packet is flowing.

`packetBytes`  

The packet’s bytes.

`packetLength`  

The length of the packet’s bytes.

## Return Value

A verdict on whether the framework should allow, drop, or delay the packet. If the verdict is NEFilterPacketProvider.Verdict.delay, the framework assumes the handler already called delayCurrentPacket(_:).

## See Also

### Filtering packets

var packetHandler: NEFilterPacketHandler?

A Swift closure or an ObjectiveC block that handles each packet received by the filter.

class NEFilterPacketContext

The context object provided to the filter packet handler.

enum NETrafficDirection

A type to represent the direction of network traffic.

enum Verdict

The verdict returned by a packet handler indicating what the framework should do with a packet.

