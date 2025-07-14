

- Network Extension
- NEPacketTunnelFlow
-  readPacketObjects(completionHandler:) 

Instance Method

# readPacketObjects(completionHandler:)

Read multiple IP packets from the TUN interface.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 17.0+visionOS 1.0+

``` source
func readPacketObjects(completionHandler: @escaping ([NEPacket]) -> Void)
```

``` source
func readPacketObjects() async -> [NEPacket]
```

## See Also

### Handling IP packets

func writePacketObjects([NEPacket]) -> Bool

Write multiple IP packets to the TUN interface.

func readPackets(completionHandler: ([Data], [NSNumber]) -> Void)

Reads IP packets from the TUN interface.

func writePackets([Data], withProtocols: [NSNumber]) -> Bool

Writes IP packets to the TUN interface.

