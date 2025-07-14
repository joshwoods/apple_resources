

- Network Extension
- NEVPNManager
-  protocol Deprecated

Instance Property

# protocol

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.11DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var `protocol`: NEVPNProtocol? { get set }
```

## Discussion

For `NEVPNManager` objects, this property can be set to either an NEVPNProtocolIPSec object or an NEVPNProtocolIKEv2 object.

## See Also

### Accessing VPN configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the VPN configuration.

var protocolConfiguration: NEVPNProtocol?

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

var localizedDescription: String?

A string containing the display name of the VPN configuration.

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

