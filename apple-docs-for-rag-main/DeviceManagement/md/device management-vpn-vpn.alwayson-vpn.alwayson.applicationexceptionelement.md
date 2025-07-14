

- Device Management
- VPN
- VPN.AlwaysOn
-  VPN.AlwaysOn.ApplicationExceptionElement 

Device Management Profile

# VPN.AlwaysOn.ApplicationExceptionElement

The dictionary that defines which applications can have traffic outside the VPN tunnel.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.AlwaysOn.ApplicationExceptionElement
```

## Properties

`BundleIdentifier`

`string`

 (Required) 

The app’s bundle identifier.

`LimitToProtocols`

`[string]`

Limit the exception to only the specified list of protocols, with support for `UDP` only.

Value: `UDP`

## See Also

### Objects

object VPN.AlwaysOn.AllowedCaptiveNetworkPluginElement

The dictionary for captive network configurations.

object VPN.AlwaysOn.ServiceExceptionElement

The dictionary that defines service exceptions.

object VPN.AlwaysOn.TunnelConfigurationElement

The dictionary used to configure VPN tunnels.

