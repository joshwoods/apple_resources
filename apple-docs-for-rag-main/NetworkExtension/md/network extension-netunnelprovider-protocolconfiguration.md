

- Network Extension
- NETunnelProvider
-  protocolConfiguration 

Instance Property

# protocolConfiguration

The configuration of the current tunneling session.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var protocolConfiguration: NEVPNProtocol { get }
```

## Discussion

The configuration is created by the containing app of the Tunnel Provider using the NETunnelProviderManager class, or by the ingestion of a `com.apple.vpn.managed` or a `com.apple.vpn.managed.applayer` configuration profile payload. See the NETunnelProviderManager class for more details.

For NEPacketTunnelProvider subclasses and NEAppProxyProvider subclasses, this property will be set to a NETunnelProviderProtocol object.

`NETunnelProvider` subclasses can observe this property using KVO to be notified when the configuration changes. For details see Key-Value Observing Programming Guide.

## See Also

### Getting the tunnel configuration

var routingMethod: NETunnelProviderRoutingMethod

The method by which network traffic is routed to the tunnel.

var appRules: [NEAppRule]?

The app rules dictating which apps use the current tunneling session.

