

- Network Extension
- NEVPNManager
-  localizedDescription 

Instance Property

# localizedDescription

A string containing the display name of the VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var localizedDescription: String? { get set }
```

## Discussion

This string is used as the display name of the VPN configuration in the system’s VPN settings UI. If this property is set to nil at the time that the configuration is created, it will be automatically set to the display name of the calling app.

## See Also

### Accessing VPN configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the VPN configuration.

var protocolConfiguration: NEVPNProtocol?

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

var `protocol`: NEVPNProtocol?

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

Deprecated

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

