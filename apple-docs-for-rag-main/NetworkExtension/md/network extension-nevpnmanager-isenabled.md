

- Network Extension
- NEVPNManager
-  isEnabled 

Instance Property

# isEnabled

A Boolean used to toggle the enabled state of the VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

A VPN configuration must be enabled before it can be used to bring up a VPN tunnel. Only one Personal VPN configuration can be enabled simultaneously on the system. If another Personal VPN configuration is enabled, then this property will be automatically set to false in the Network Extension preferences. Note that you will need to re-load the VPN configuration from the preferences in order to see the change in value. You can register with NotificationCenter to observe the NEVPNConfigurationChangeNotification notification for the NEVPNManager object so that your code can detect when the VPN configuration has been disabled.

## See Also

### Accessing VPN configuration properties

var protocolConfiguration: NEVPNProtocol?

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

var `protocol`: NEVPNProtocol?

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

Deprecated

var localizedDescription: String?

A string containing the display name of the VPN configuration.

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

