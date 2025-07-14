

- Network Extension
- NEVPNProtocol
-  enforceRoutes 

Instance Property

# enforceRoutes

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

iOS 14.2+iPadOS 14.2+Mac Catalyst 14.2+macOS 11.0+tvOS 17.0+visionOS 1.0+

``` source
var enforceRoutes: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If this property is true when the includeAllNetworks property is false, the system scopes the included routes to the VPN and the excluded routes to the current primary network interface. This property supersedes the system routing table and scoping operations by apps.

If you set both the enforceRoutes and excludeLocalNetworks properties to true, the system excludes network connections to hosts on the local network.

NETransparentProxyManager doesn’t support this property. The default value for this property is false.

Note

You specify the included and excluded routes using the respective `includedRoutes` and `excludedRoutes` properties in the NEIPv4Settings and NEIPv6Settings objects that you provide in the NEPacketTunnelProvider settings.

## See Also

### Routing network traffic

var includeAllNetworks: Bool

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

var excludeAPNs: Bool

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

var excludeCellularServices: Bool

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

var excludeLocalNetworks: Bool

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

