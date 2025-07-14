

- Network Extension
- NEVPNManager
-  onDemandRules 

Instance Property

# onDemandRules

An ordered list of Connect On Demand rules.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var onDemandRules: [NEOnDemandRule]? { get set }
```

## Discussion

The VPN configuration can optionally be configured to connect automatically based on a variety of criteria specified in NEOnDemandRule objects. The onDemandRules property contains the current set of Connect On Demand rules for the VPN configuration. Each rule is evaluated in order, and the first rule that matches all criteria on the current network is applied.

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

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

