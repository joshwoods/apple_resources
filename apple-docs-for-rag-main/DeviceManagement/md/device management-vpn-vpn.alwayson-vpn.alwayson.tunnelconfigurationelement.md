

- Device Management
- VPN
- VPN.AlwaysOn
-  VPN.AlwaysOn.TunnelConfigurationElement 

Device Management Profile

# VPN.AlwaysOn.TunnelConfigurationElement

The dictionary used to configure VPN tunnels.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.AlwaysOn.TunnelConfigurationElement
```

## Properties

`Interfaces`

`[string]`

The interfaces to apply this configuration to.

Possible Values: `Cellular, WiFi`

`ProtocolType`

`string`

 (Required) 

The type of connection, which needs to be `IKEv2`.

Value: `IKEv2`

## See Also

### Objects

object VPN.AlwaysOn.AllowedCaptiveNetworkPluginElement

The dictionary for captive network configurations.

object VPN.AlwaysOn.ApplicationExceptionElement

The dictionary that defines which applications can have traffic outside the VPN tunnel.

object VPN.AlwaysOn.ServiceExceptionElement

The dictionary that defines service exceptions.

