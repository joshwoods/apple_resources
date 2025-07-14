

- Device Management
- VPN
-  VPN.IPSec 

Device Management Profile

# VPN.IPSec

The dictionary to use for an IPSec VPN type.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.IPSec
```

## Properties

`AuthenticationMethod`

`string`

The authentication method for L2TP and Cisco IPSec.

Default: `SharedSecret`

Possible Values: `SharedSecret, Certificate`

`DisconnectOnIdle`

`integer`

If `1`, disconnect after an on-demand connection idles.

Default: `0`

Possible Values: `0, 1`

`DisconnectOnIdleTimer`

`integer`

The length of time to wait before disconnecting an on-demand connection.

`LocalIdentifier`

`string`

The name of the group. For hybrid authentication, the string needs to end with “hybrid”.

Present only for Cisco IPSec if `AuthenticationMethod` is `SharedSecret`.

`LocalIdentifierType`

`string`

Present only if `AuthenticationMethod` is `SharedSecret`. The value is `KeyID`. The system uses this value for L2TP and Cisco IPSec VPNs.

Value: `KeyID`

`OnDemandEnabled`

`integer`

If `1`, enables bringing the VPN connection up on demand.

Default: `0`

Possible Values: `0, 1`

`OnDemandRules`

`[`VPN.VPN.OnDemandRulesElement`]`

The on-demand rules dictionary.

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for the account credentials.

Only use this with Cisco IPSec VPNs and if the `AuthenticationMethod` key is to `Certificate`.

`PromptForVPNPIN`

`boolean`

If `true`, prompts for a PIN when connecting to Cisco IPSec VPNs.

Default: `false`

`RemoteAddress`

`string`

The IP address or host name of the VPN server.

`SharedSecret`

`data`

The shared secret for this VPN account.

Only use this with L2TP and Cisco IPSec VPNs and if the `AuthenticationMethod` key is to `SharedSecret`.

`XAuthEnabled`

`integer`

If `1`, enables Xauth for Cisco IPSec VPNs.

Possible Values: `0, 1`

`XAuthName`

`string`

The user name for the VPN account for Cisco IPSec.

`XAuthPassword`

`string`

The VPN account password for Cisco IPSec.

`XAuthPasswordEncryption`

`string`

A string that either has the value “Prompt” or isn’t present.

Value: `Prompt`

`OnDemandMatchDomainsAlways`

`[string]`

Deprecated 

Deprecated. A list of domain names. In iOS 7 and later, if this key is present, the system treats associated domain names as though they’re associated with the `OnDemandMatchDomainsOnRetry` key. This behavior can be overridden by `OnDemandRules`.

`OnDemandMatchDomainsOnRetry`

`[string]`

Deprecated 

Deprecated. A list of domain names. In iOS 7 and later, this field is deprecated (but still supported) in favor of `EvaluateConnection` actions in the `OnDemandRules` dictionaries.

`OnDemandMatchDomainsNever`

`[string]`

Deprecated 

Deprecated. A list of domain names. In iOS 7 and later, this key is deprecated (but still supported) in favor of `EvaluateConnection` actions in the `OnDemandRules` dictionaries.

## Discussion

The system uses this dictionary when the `VPNType` is `IPSec`.

## See Also

### Profiles

object VPN.AlwaysOn

The dictionary that contains IPSec settings.

object VPN.DNS

The dictionary to configure DNS settings for the VPN.

object VPN.IKEv2

The dictionary to use for an IKEv2 VPN type.

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

