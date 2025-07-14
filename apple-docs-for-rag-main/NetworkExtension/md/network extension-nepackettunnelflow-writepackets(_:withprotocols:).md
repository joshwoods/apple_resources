

- Network Extension
- NEPacketTunnelFlow
-  writePackets(\_:withProtocols:) 

Instance Method

# writePackets(\_:withProtocols:)

Writes IP packets to the TUN interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
func writePackets(
    _ packets: [Data],
    withProtocols protocols: [NSNumber]
) -> Bool
```

## Parameters 

`packets`  

An array of NSData objects containing the IP packets to the written.

`protocols`  

An array of NSNumber objects containing the protocol numbers (e.g. AF_INET or AF_INET6) of the IP packets in `packets` in host byte order.

## Discussion

The number of NSData objects in `packets` must be exactly equal to the number of NSNumber objects in `protocols`.

## See Also

### Handling IP packets

func readPacketObjects(completionHandler: ([NEPacket]) -> Void)

Read multiple IP packets from the TUN interface.

func writePacketObjects([NEPacket]) -> Bool

Write multiple IP packets to the TUN interface.

func readPackets(completionHandler: ([Data], [NSNumber]) -> Void)

Reads IP packets from the TUN interface.

