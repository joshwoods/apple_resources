

- Network Extension
- NEVPNProtocol
-  excludeAPNs 

Instance Property

# excludeAPNs

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var excludeAPNs: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If this property is true, the system excludes Apple Push Notification services (APNs) traffic, but only when the includeAllNetworks property is also true. NETransparentProxyManager doesn’t support this property.

The default value for this property is true.

## See Also

### Routing network traffic

var includeAllNetworks: Bool

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

var excludeCellularServices: Bool

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

var excludeLocalNetworks: Bool

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

var enforceRoutes: Bool

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

