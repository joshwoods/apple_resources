

- Device Management
- VPN
-  VPN.VPN 

Device Management Profile

# VPN.VPN

The dictionary that contains VPN, IPSec, and IKEv2 settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 17.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object VPN.VPN
```

## Properties

`AuthName`

`string`

`AuthPassword`

`string`

`AuthenticationMethod`

`string`

The authentication method to use.

Default: `Password`

Possible Values: `Password, Certificate, Password+Certificate`

`DisconnectOnIdle`

`integer`

If `1`, disconnects after an on-demand connection idles.

Default: `0`

Possible Values: `0, 1`

`DisconnectOnIdleTimer`

`integer`

The length of time to wait, in seconds, before disconnecting an on-demand connection. In watchOS, the maximum allowed value is `15`.

`EnforceRoutes`

`integer`

If `1`, all the VPN’s non-default routes take precedence over any locally defined routes.

If `IncludeAllNetworks` is `1`, the system ignores the value of `EnforceRoutes`.

Available in iOS 14.2 and later, and macOS 11 and later. Not available in watchOS.

Default: `0`

Possible Values: `0, 1`

`ExcludeAPNs`

`integer`

If `1` and `IncludeAllNetworks` is `1`, then the system excludes the network traffic for the Apple Push Notification service (APNs) from the tunnel. Not available in watchOS.

Default: `1`

Possible Values: `0, 1`

`ExcludeCellularServices`

`integer`

If `1` and `IncludeAllNetworks` is `1`, then the system excludes internet-routable network traffic for cellular services (VoLTE, Wi-Fi Calling, IMS, MMS, Visual Voicemail, etc.) from the tunnel. Note that some cellular carriers route cellular services traffic directly to the carrier network, bypassing the internet. Such cellular services traffic is always excluded from the tunnel. Not available in watchOS.

Default: `1`

Possible Values: `0, 1`

`ExcludeDeviceCommunication`

`integer`

Default: `1`

Possible Values: `0, 1`

`ExcludeLocalNetworks`

`integer`

If `1` and `IncludeAllNetworks` is `1`, routes all local network traffic outside the VPN. Not available in watchOS.

Possible Values: `0, 1`

`IncludeAllNetworks`

`integer`

If `1`, routes all traffic through the VPN. Not available in watchOS.

Default: `0`

Possible Values: `0, 1`

`OnDemandEnabled`

`integer`

If `1`, enables VPN On Demand.

Default: `0`

Possible Values: `0, 1`

`OnDemandMatchDomainsAlways`

`[string]`

Deprecated 

A list of domain names. The system treats associated domain names as though they’re associated with the `OnDemandMatchDomainsOnRetry` key. This behavior can be overridden by `OnDemandRules`.

In iOS 7 and later, this key is deprecated (but still supported) in favor of `EvaluateConnection` actions in the `OnDemandRules` dictionaries.

Not available in watchOS.

`OnDemandMatchDomainsNever`

`[string]`

Deprecated 

A list of domain names. If the host name ends with one of these domain names, the system doesn’t start the VPN automatically. The system uses this value to exclude a subdomain within an included domain.

In iOS 7 and later, this key is deprecated (but still supported) in favor of `EvaluateConnection` actions in the `OnDemandRules` dictionaries.

Not available in watchOS.

`OnDemandMatchDomainsOnRetry`

`[string]`

Deprecated 

A list of domain names. If the host name ends with one of these domain names and a DNS query for that domain name fails, the system starts the VPN automatically.

In iOS 7 and later, this key is deprecated (but still supported) in favor of `EvaluateConnection` actions in the `OnDemandRules` dictionaries.

Not available in watchOS.

`OnDemandRules`

`[`VPN.VPN.OnDemandRulesElement`]`

An array of dictionaries defining On Demand Rules.

`OnDemandUserOverrideDisabled`

`integer`

If `1`, the Connect On Demand toggle in Settings is disabled for this configuration. Available in iOS 14 and later. Not available in watchOS.

Default: `0`

Possible Values: `0, 1`

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for account credentials.

`ProviderBundleIdentifier`

`string`

The bundle identifier for the VPN provider. Not available in watchOS.

`ProviderDesignatedRequirement`

`string`

If the VPN provider is implemented as a system extension, this field is required. Not available in watchOS.

`ProviderType`

`string`

The type of VPN service. If the value is `app-proxy`, the service tunnels traffic at the app level. If the value is `packet-tunnel`, the service tunnels traffic at the IP layer. Not available in watchOS.

Default: `packet-tunnel`

Possible Values: `packet-tunnel, app-proxy`

`RemoteAddress`

`string`

 (Required) 

## Discussion

The system uses this dictionary when the `VPNType` is `VPN`, `IPSec`, or `IKEv2`.

## Topics

### Objects

object VPN.VPN.OnDemandRulesElement

The dictionary that contains settings for On Demand connections.

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

object VPN.TransparentProxy

The dictionary to use for a transparent proxy VPN type.

object VPN.VendorConfig

The vendor-specific configuration dictionary.

