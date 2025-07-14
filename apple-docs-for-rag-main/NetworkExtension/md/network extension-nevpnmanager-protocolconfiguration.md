

- Network Extension
- NEVPNManager
-  protocolConfiguration 

Instance Property

# protocolConfiguration

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var protocolConfiguration: NEVPNProtocol? { get set }
```

## Discussion

For `NEVPNManager` objects, this property can be set to either an NEVPNProtocolIPSec object or an NEVPNProtocolIKEv2 object.

## See Also

### Accessing VPN configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the VPN configuration.

var `protocol`: NEVPNProtocol?

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

Deprecated

var localizedDescription: String?

A string containing the display name of the VPN configuration.

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

