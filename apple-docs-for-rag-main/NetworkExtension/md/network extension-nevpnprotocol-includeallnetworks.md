

- Network Extension
- NEVPNProtocol
-  includeAllNetworks 

Instance Property

# includeAllNetworks

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
var includeAllNetworks: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

If this property is true, the system routes network traffic through the tunnel except traffic for designated system services necessary for maintaining expected device functionality.

You can exclude some types of traffic using the excludeAPNs, excludeLocalNetworks, and excludeCellularServices properties in combination with this property. The system always excludes the following network traffic from the tunnel regardless of this property value:

- Network control plane traffic that maintains a device’s connection to the local network, such as DHCP.

- Captive portal negotiation traffic that authorizes a device with a Wi-Fi hotspot.

- Certain cellular services traffic that uses the cellular network only, such as VoLTE.

- Traffic that communicates with a companion device, such as an Apple Watch.

NETransparentProxyManager doesn’t support this property. The default value for this property is false.

## See Also

### Routing network traffic

var excludeAPNs: Bool

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

var excludeCellularServices: Bool

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

var excludeLocalNetworks: Bool

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

var enforceRoutes: Bool

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

