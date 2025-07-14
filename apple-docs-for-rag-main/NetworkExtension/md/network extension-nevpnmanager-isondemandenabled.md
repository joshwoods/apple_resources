

- Network Extension
- NEVPNManager
-  isOnDemandEnabled 

Instance Property

# isOnDemandEnabled

A Boolean used to toggle the Connect On Demand capability.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var isOnDemandEnabled: Bool { get set }
```

## Mentioned in 

Routing your VPN network traffic

## Discussion

The default value of this property is false.

## See Also

### Accessing VPN configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the VPN configuration.

var protocolConfiguration: NEVPNProtocol?

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

var `protocol`: NEVPNProtocol?

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

Deprecated

var localizedDescription: String?

A string containing the display name of the VPN configuration.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

