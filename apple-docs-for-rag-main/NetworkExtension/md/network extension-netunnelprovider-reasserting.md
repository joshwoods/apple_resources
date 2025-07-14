

- Network Extension
- NETunnelProvider
-  reasserting 

Instance Property

# reasserting

Indicate to the system that the tunnel is being re-established.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var reasserting: Bool { get set }
```

## Discussion

The Tunnel Provider should set this property to true whenever it starts to reconnect to the tunnel server. Once the Tunnel Provider completes the process of reconnecting it should set this property to false.

