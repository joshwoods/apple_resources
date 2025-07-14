

- Device Management
- VPN
-  VPN.AlwaysOn 

Device Management Profile

# VPN.AlwaysOn

The dictionary that contains IPSec settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.AlwaysOn
```

## Properties

`AllowAllCaptiveNetworkPlugins`

`integer`

If `1`, allows traffic from all captive networking apps outside the VPN tunnel to perform captive network handling.

Default: `0`

Possible Values: `0, 1`

`AllowCaptiveWebSheet`

`integer`

If `1`, allows traffic from Captive Web Sheet outside the VPN tunnel.

Default: `0`

Possible Values: `0, 1`

`AllowedCaptiveNetworkPlugins`

`[`VPN.AlwaysOn.AllowedCaptiveNetworkPluginElement`]`

The array of captive networking apps whose traffic is allowed outside the VPN tunnel, to perform captive network handling. Used only when `AllowAllCaptiveNetworkPlugins` is `false`.

`ApplicationExceptions`

`[`VPN.AlwaysOn.ApplicationExceptionElement`]`

An array that contains an arbitrary number of apps whose connections occur outside the VPN.

`ServiceExceptions`

`[`VPN.AlwaysOn.ServiceExceptionElement`]`

An array that contains an arbitrary number of service exceptions.

`TunnelConfigurations`

`[`VPN.AlwaysOn.TunnelConfigurationElement`]`

 (Required) 

An array that contains an arbitrary number of tunnel configurations.

`UIToggleEnabled`

`integer`

If `1`, allows the user to disable the VPN configuration.

Default: `0`

Possible Values: `0, 1`

## Discussion

The system uses this dictionary when the `VPNType` is `AlwaysOn`.

## Topics

### Objects

object VPN.AlwaysOn.AllowedCaptiveNetworkPluginElement

The dictionary for captive network configurations.

object VPN.AlwaysOn.ApplicationExceptionElement

The dictionary that defines which applications can have traffic outside the VPN tunnel.

object VPN.AlwaysOn.ServiceExceptionElement

The dictionary that defines service exceptions.

object VPN.AlwaysOn.TunnelConfigurationElement

The dictionary used to configure VPN tunnels.

## See Also

### Profiles

object VPN.DNS

The dictionary to configure DNS settings for the VPN.

object VPN.IKEv2

The dictionary to use for an IKEv2 VPN type.

object VPN.IPSec

The dictionary to use for an IPSec VPN type.

object VPN.IPv4

The dictionary that contains IPV4 settings.

object VPN.PPP

The dictionary that contains PPP settings.

object VPN.Proxies

The dictionary that contains the Proxies settings.

object VPN.VPN

The dictionary that contains VPN, IPSec, and IKEv2 settings.

object VPN.TransparentProxy

The dictionary to use for a transparent proxy VPN type.

object VPN.VendorConfig

The vendor-specific configuration dictionary.

