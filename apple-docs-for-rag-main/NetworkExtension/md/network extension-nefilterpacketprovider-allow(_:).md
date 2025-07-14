

- Network Extension
- NEFilterPacketProvider
-  allow(\_:) 

Instance Method

# allow(\_:)

Allow delivery of a previously-delayed packet.

macOS 10.15+

``` source
func allow(_ packet: NEPacket)
```

## Parameters 

`packet`  

The packet previously delayed by the packet handler.

## Discussion

Use this method to allow a previously-delayed packet to continue its journey into or out of the networking stack.

## See Also

### Delaying packets

func delayCurrentPacket(NEFilterPacketContext) -> NEPacket

Delay a packet currently processed by a packet handler.

