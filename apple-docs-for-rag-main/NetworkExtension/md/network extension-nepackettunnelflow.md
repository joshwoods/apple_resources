

- Network Extension
-  NEPacketTunnelFlow 

Class

# NEPacketTunnelFlow

An object you use to read and write packets to and from the tunnel’s virtual interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEPacketTunnelFlow
```

## Overview

Use the `NEPacketTunnelFlow` class to implement a custom-IP tunneling protocol for your packet tunnel. For example, use the APIs in this class to read packets from the virtual interface, so you can then encapsulate these packets and send them to a packet-tunnel server. Likewise, read packets from your packet-tunnel server and use these APIs to write the packets back to the tunnel’s virtual interface.

## Topics

### Handling IP packets

func readPacketObjects(completionHandler: ([NEPacket]) -> Void)

Read multiple IP packets from the TUN interface.

func writePacketObjects([NEPacket]) -> Bool

Write multiple IP packets to the TUN interface.

func readPackets(completionHandler: ([Data], [NSNumber]) -> Void)

Reads IP packets from the TUN interface.

func writePackets([Data], withProtocols: [NSNumber]) -> Bool

Writes IP packets to the TUN interface.

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

### Packet handling

class NEPacket

A network packet and its associated properties.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

