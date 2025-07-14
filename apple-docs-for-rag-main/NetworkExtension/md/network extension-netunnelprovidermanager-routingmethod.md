

- Network Extension
- NETunnelProviderManager
-  routingMethod 

Instance Property

# routingMethod

The method that the system uses to route network traffic to the tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var routingMethod: NETunnelProviderRoutingMethod { get }
```

## Discussion

The default is NETunnelProviderRoutingMethod.destinationIP.

## See Also

### Getting tunnel configuration properties

enum NETunnelProviderRoutingMethod

