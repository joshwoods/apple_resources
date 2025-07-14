

- Network Extension
- NEPacketTunnelProvider
-  packetFlow 

Instance Property

# packetFlow

A NEPacketTunnelFlow object which is used to receive IP packets routed to the tunnel’s virtual interface and inject IP packets into the networking stack via the tunnel’s virtual interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var packetFlow: NEPacketTunnelFlow { get }
```

