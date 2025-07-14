

- Network Extension
- NEPacketTunnelFlow
-  writePacketObjects(\_:) 

Instance Method

# writePacketObjects(\_:)

Write multiple IP packets to the TUN interface.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 17.0+visionOS 1.0+

``` source
func writePacketObjects(_ packets: [NEPacket]) -> Bool
```

## See Also

### Handling IP packets

func readPacketObjects(completionHandler: ([NEPacket]) -> Void)

Read multiple IP packets from the TUN interface.

func readPackets(completionHandler: ([Data], [NSNumber]) -> Void)

Reads IP packets from the TUN interface.

func writePackets([Data], withProtocols: [NSNumber]) -> Bool

Writes IP packets to the TUN interface.

