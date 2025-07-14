

- Network Extension
-  NETunnelProviderRoutingMethod 

Enumeration

# NETunnelProviderRoutingMethod

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
enum NETunnelProviderRoutingMethod
```

## Topics

### Routing Methods

case destinationIP

Route network traffic to the tunnel based on destination IP.

case sourceApplication

Route network traffic to the tunnel based on source application.

case networkRule

A routing method that routes traffic based on network rule objects specified by the provider.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting tunnel configuration properties

var routingMethod: NETunnelProviderRoutingMethod

The method that the system uses to route network traffic to the tunnel.

