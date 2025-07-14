

- Network Extension
- NEVPNProtocol
-  excludeCellularServices 

Instance Property

# excludeCellularServices

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var excludeCellularServices: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If this property is true, the system excludes cellular services — such as Wi-Fi Calling, MMS, SMS, and Visual Voicemail — but only when the includeAllNetworks property is also true. This property doesn’t impact services that use the cellular network only — such as VoLTE — which the system automatically excludes. NETransparentProxyManager doesn’t support this property.

The default value for this property is true.

## See Also

### Routing network traffic

var includeAllNetworks: Bool

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

var excludeAPNs: Bool

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

var excludeLocalNetworks: Bool

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

var enforceRoutes: Bool

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

