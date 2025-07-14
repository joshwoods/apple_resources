

- Network Extension
- NEFilterPacketProvider
-  delayCurrentPacket(\_:) 

Instance Method

# delayCurrentPacket(\_:)

Delay a packet currently processed by a packet handler.

macOS 10.15+

``` source
func delayCurrentPacket(_ context: NEFilterPacketContext) -> NEPacket
```

## Parameters 

`context`  

A context for the packet handler.

## Discussion

This function is only valid within the packetHandler Swift closure or ObjectiveC block, which must return NEFilterPacketProvider.Verdict.delay after delaying the packet. The framework prevents further delivery of the packet through the network stack until it’s allowed or dropped. Allow the packet by calling allow(_:), or drop it by releasing it.

## See Also

### Delaying packets

func allow(NEPacket)

Allow delivery of a previously-delayed packet.

