

- Network Extension
- NEVPNProtocol
-  excludeLocalNetworks 

Instance Property

# excludeLocalNetworks

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

iOS 14.2+iPadOS 14.2+Mac Catalyst 14.2+macOS 10.15+visionOS 1.0+

``` source
var excludeLocalNetworks: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If this property is true, the system excludes network connections to hosts on the local network — such as AirPlay, AirDrop, and CarPlay — but only when the includeAllNetworks or enforceRoutes property is also true. NETransparentProxyManager doesn’t support this property.

The default value for this property is false in macOS and true in iOS`.`

## See Also

### Routing network traffic

var includeAllNetworks: Bool

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

var excludeAPNs: Bool

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

var excludeCellularServices: Bool

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

var enforceRoutes: Bool

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

