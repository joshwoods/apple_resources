

- Device Management
- VPN
-  VPN.IPv4 

Device Management Profile

# VPN.IPv4

The dictionary that contains IPV4 settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.IPv4
```

## Properties

`OverridePrimary`

`integer`

If `1`, the system sends all network traffic over VPN.

Default: `0`

Possible Values: `0, 1`

## See Also

### Profiles

object VPN.AlwaysOn

The dictionary that contains IPSec settings.

object VPN.DNS

The dictionary to configure DNS settings for the VPN.

object VPN.IKEv2

The dictionary to use for an IKEv2 VPN type.

object VPN.IPSec

The dictionary to use for an IPSec VPN type.

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

