

- Device Management
-  VPN 

Device Management Profile

# VPN

The payload you use to configure a VPN.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN
```

## Properties

`AlwaysOn`

VPN.AlwaysOn

The dictionary to use when `VPNType` is `AlwaysOn`. Not available in tvOS or watchOS.

`DNS`

VPN.DNS

A dictionary to use for all VPN types.

`IKEv2`

VPN.IKEv2

The dictionary to use when `VPNType` is `IKEv2`.

`IPSec`

VPN.IPSec

The dictionary that contains IPSec settings. Not available in watchOS.

`IPv4`

VPN.IPv4

The dictionary that contains IPv4 settings. Not available in watchOS.

`PPP`

VPN.PPP

The dictionary to use when `VPNType` is `L2TP` or `PTPP`. Not available in watchOS.

`Proxies`

VPN.Proxies

The dictionary to use to configure `Proxies` for use with `VPN`.

`TransparentProxy`

VPN.TransparentProxy

The dictionary to use when `VPNType` is `TransparentProxy`. Available in macOS 14 and later.

`UserDefinedName`

`string`

 (Required) 

The description of the VPN connection that the system displays on the device. Not available in watchOS.

`VendorConfig`

VPN.VendorConfig

The vendor-specific configuration dictionary, which the system reads only when `VPNSubType` has a value. Not available in watchOS.

`VPN`

VPN.VPN

The dictionary to use to specify a VPN when `VPNType` is `VPN`, `IPSec`, or `IKEv2`.

`VPNSubType`

`string`

An identifier for a vendor-specified configuration dictionary when the value for `VPNType` is `VPN`.

If `VPNType` is `VPN`, the system requires this field. If the configuration targets a VPN solution that uses a VPN plugin, then this field contains the bundle identifier of the plugin. Here are some examples:

- Cisco AnyConnect: `com.cisco.anyconnect.applevpn.plugin`

- Juniper SSL: `net.juniper.sslvpn`

- F5 SSL: `com.f5.F5-Edge-Client.vpnplugin`

- SonicWALL Mobile Connect: `com.sonicwall.SonicWALL-SSLVPN.vpnplugin`

- \`\`Aruba VIA: `com.arubanetworks.aruba-via.vpnplugin`

If the configuration targets a VPN solution that uses a network extension provider, then this field contains the bundle identifier of the app that contains the provider. Contact the VPN solution vendor for the value of the identifier.

If `VPNType` is `IKEv2`, then the `VPNSubType` field is optional and reserved for future use. If it’s specified, it needs to contain an empty string.

Not available in watchOS.

`VPNType`

`string`

 (Required) 

The type of the VPN, which defines which settings are appropriate for this VPN payload.

If the type is `VPN` or `TransparentProxy`, then the system requires a value for `VPNSubType`.

`TransparentProxy` is only available in macOS. `L2TP` and `IPSec` aren’t available in tvOS. `AlwaysOn` is only available on iOS and Apple Watch pairing isn’t supported with `AlwaysOn`. For a previously paired Apple Watch, all phone-watch communications cease when `AlwaysOn` is enabled. Not available in watchOS.

Possible Values: `VPN, L2TP, IPSec, IKEv2, AlwaysOn, TransparentProxy`

## Discussion

Specify `com.apple.vpn.managed` as the payload type.

### Profile Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | macOS                         |
| Allow Manual Install       | iOS, macOS, tvOS              |
| Requires Supervision       | \-                            |
| Requires User Approved MDM | \-                            |
| Allowed in User Enrollment | \-                            |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS |

### Profile Example

```

    PayloadContent

            IPSec

                AuthenticationMethod
                SharedSecret
                LocalIdentifierType
                KeyID
                SharedSecret

                UVhCd2JHVXhNak1o

            IPv4

                OverridePrimary
                0

            PPP

                AuthName
                username
                AuthPassword
                password
                CommRemoteAddress
                vpn.example.com

            Proxies

                HTTPEnable
                0
                HTTPSEnable
                0

            UserDefinedName
            VPN Server
            VPNType
            L2TP
            PayloadIdentifier
            com.example.myvpnmanagedprofile
            PayloadType
            com.apple.vpn.managed
            PayloadUUID
            74615F25-3B51-4386-A31B-ACB1F1094EF9
            PayloadVersion
            1

    PayloadDisplayName
    VPN
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    01E7F1C0-2DD0-4E36-82FF-EC6F29BB6C45
    PayloadVersion
    1

```

## Topics

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

object VPN.VendorConfig

The vendor-specific configuration dictionary.

## See Also

### VPN

object AppLayerVPN

The payload you use to configure add-on VPN software.

object AppToAppLayerVPNMapping

The payload you use to configure per-app VPN settings.

