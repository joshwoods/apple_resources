

- Network Extension
- NEIPv6Settings
-  includedRoutes 

Instance Property

# includedRoutes

The IPv6 network traffic that the system routes to the TUN interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var includedRoutes: [NEIPv6Route]? { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If you include the default route (`0.0.0.0/0` or `::/0`) in this property, the system routes traffic that doesn’t match a specific rule in the system routing table through the VPN.

## See Also

### Routing network traffic

var excludedRoutes: [NEIPv6Route]?

The IPv6 network traffic that the system routes to the primary physical interface, not the TUN interface.

class NEIPv6Route

The settings for an IPv6 route.

