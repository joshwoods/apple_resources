

- Network Extension
- NETunnelProvider
-  routingMethod 

Instance Property

# routingMethod

The method by which network traffic is routed to the tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var routingMethod: NETunnelProviderRoutingMethod { get }
```

## Discussion

The default is NETunnelProviderRoutingMethod.destinationIP.

## See Also

### Getting the tunnel configuration

var protocolConfiguration: NEVPNProtocol

The configuration of the current tunneling session.

var appRules: [NEAppRule]?

The app rules dictating which apps use the current tunneling session.

