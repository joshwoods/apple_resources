

- Network Extension
- NEIPv4Settings
-  excludedRoutes 

Instance Property

# excludedRoutes

The IPv4 network traffic that the system routes to the primary physical interface, not the TUN interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var excludedRoutes: [NEIPv4Route]? { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

This property excludes routes that the system might otherwise include from the includedRoutes property. The system automatically excludes the IP address of the tunnel server.

## See Also

### Routing network traffic

var includedRoutes: [NEIPv4Route]?

The IPv4 network traffic that the system routes to the TUN interface.

class NEIPv4Route

The settings for an IPv4 route.

