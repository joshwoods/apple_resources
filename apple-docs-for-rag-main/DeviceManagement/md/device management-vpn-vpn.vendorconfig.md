

- Device Management
- VPN
-  VPN.VendorConfig 

Device Management Profile

# VPN.VendorConfig

The vendor-specific configuration dictionary.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.VendorConfig
```

## Properties

`Group`

`string`

The group to connect to on the head end. Valid for Cisco AnyConnect and Cisco Legacy AnyConnect.

`LoginGroupOrDomain`

`string`

The login group or domain. Valid only for SonicWALL Mobile Connect.

`Realm`

`string`

The Kerberos realm name, which needs to be properly capitalized. Valid only for Juniper SSL and Pulse Secure.

`Role`

`string`

The role to select when connecting to the server. Valid only for Juniper SSL and Pulse Secure.

## Discussion

The system only reads this value when `VPNSubType` has a value. Contact your VPN solution vendor for information about what keys you can configure in this dictionary.

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

