

- Network Extension
- NETunnelProvider
-  appRules 

Instance Property

# appRules

The app rules dictating which apps use the current tunneling session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var appRules: [NEAppRule]? { get }
```

## Discussion

This property is only non-`nil` if the current configuration is a Per-App VPN configuration.

## See Also

### Getting the tunnel configuration

var protocolConfiguration: NEVPNProtocol

The configuration of the current tunneling session.

var routingMethod: NETunnelProviderRoutingMethod

The method by which network traffic is routed to the tunnel.

