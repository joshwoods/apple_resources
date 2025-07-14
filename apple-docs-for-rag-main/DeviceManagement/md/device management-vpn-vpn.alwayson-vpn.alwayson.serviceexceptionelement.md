

- Device Management
- VPN
- VPN.AlwaysOn
-  VPN.AlwaysOn.ServiceExceptionElement 

Device Management Profile

# VPN.AlwaysOn.ServiceExceptionElement

The dictionary that defines service exceptions.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.AlwaysOn.ServiceExceptionElement
```

## Properties

`Action`

`string`

 (Required) 

The action to take with network connections from the named service.

Possible Values: `Allow, Drop`

`ServiceName`

`string`

 (Required) 

The name of a service that’s exempt from Always On VPN. `CellularServices` is available in iOS 11.3 and later; it exempts `VoLTE`, `IMS` and `MMS`. WiFiCalling is exempted in iOS 13.4 and later.

Possible Values: `VoiceMail, AirPrint, CellularServices, DeviceCommunication`

## See Also

### Objects

object VPN.AlwaysOn.AllowedCaptiveNetworkPluginElement

The dictionary for captive network configurations.

object VPN.AlwaysOn.ApplicationExceptionElement

The dictionary that defines which applications can have traffic outside the VPN tunnel.

object VPN.AlwaysOn.TunnelConfigurationElement

The dictionary used to configure VPN tunnels.

