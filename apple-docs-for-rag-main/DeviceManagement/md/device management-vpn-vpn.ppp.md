

- Device Management
- VPN
-  VPN.PPP 

Device Management Profile

# VPN.PPP

The dictionary that contains PPP settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.PPP
```

## Properties

`AuthEAPPlugins`

`[string]`

An array of authentication plugins. For use of RSA SecurID, this array should only have one value: `EAP-RSA`. This key is for use with L2TP and PPTP networks.

Possible Values: `EAP-RSA, EAP-TLS, EAP-KRB`

`AuthName`

`string`

The VPN account user name. This key is for use with L2TP and PPTP networks.

`AuthPassword`

`string`

If `TokenCard` is `1`, use this password for authentication. This keyis for use with L2TP and PPTP networks.

`AuthProtocol`

`[string]`

An array of authentication protocols. For use of RSA SecurID, this array should have one value, `EAP`. This key is for use with L2TP and PPTP networks.

Value: `EAP`

`CCPEnabled`

`integer`

If `1`, enables encryption on the connection. This key is for use with PPTP networks.

Possible Values: `0, 1`

`CCPMPPE128Enabled`

`integer`

If `1` and `CCPEnabled` is also `1`, enables CCPMPPE40 encryption.

Possible Values: `0, 1`

`CCPMPPE40Enabled`

`integer`

If `1` and `CCPEnabled` is also `1`, enables CCPMPPE128 encryption.

Possible Values: `0, 1`

`CommRemoteAddress`

`string`

The IP address or host name of VPN server. This key is for use with L2TP and PPTP networks.

`DisconnectOnIdle`

`integer`

If `1`, disconnects after an on demand connection idles.

Default: `0`

Possible Values: `0, 1`

`DisconnectOnIdleTimer`

`integer`

The length of time to wait before disconnecting an on demand connection

`TokenCard`

`integer`

If `1`, uses a token card such as an RSA SecurID card for connecting. This key is for use with L2TP networks.

Default: `0`

Possible Values: `0, 1`

## Discussion

The system uses this dictionary when the `VPNType` is `L2TP` or `PTPP`.

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

object VPN.Proxies

The dictionary that contains the Proxies settings.

object VPN.VPN

The dictionary that contains VPN, IPSec, and IKEv2 settings.

object VPN.TransparentProxy

The dictionary to use for a transparent proxy VPN type.

object VPN.VendorConfig

The vendor-specific configuration dictionary.

