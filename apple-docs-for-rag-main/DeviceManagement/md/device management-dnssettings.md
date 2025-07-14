

- Device Management
-  DNSSettings 

Device Management Profile

# DNSSettings

The payload you use to configure encrypted DNS settings.

iOS 14.0+iPadOS 14.0+macOS 11.0+visionOS 1.0+Device Assignment ServicesVPP License Management

``` source
object DNSSettings
```

## Properties

`DNSSettings`

DNSSettings.DNSSettings

 (Required) 

A dictionary that defines a configuration for an encrypted DNS server.

`OnDemandRules`

`[`DNSSettings.OnDemandRulesElement`]`

An array of rules that define the DNS settings. If not set, the system always applies the DNS settings. These rules are identical to the `OnDemandRules` array in VPN payloads.

`PayloadCertificateUUID`

`string`

The UUID that points to an identity certificate payload. The system uses this identity to authenticate the user to the DNS resolver.

`ProhibitDisablement`

`boolean`

If `true`, the system prohibits users from disabling DNS settings. This key is only available on supervised devices.

Default: `false`

## Discussion

Specify `com.apple.dnsSettings.managed` as the payload type.

When installed from an MDM, the setting only applies to managed wifi networks

When installed manually, this setting also applies to cellular.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | \-                      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User-Approved MDM | \-                      |
| Allowed in User Enrollment | \-                      |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad |

## Topics

### Objects

object DNSSettings.DNSSettings

A dictionary that defines a configuration for an encrypted DNS server.

object DNSSettings.OnDemandRulesElement

A list of domain strings that determine which DNS queries use the DNS server.

## See Also

### Networking

object Cellular

The payload you use to configure cellular settings.

object CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

object ContentCaching

The payload you use to configure the content-caching service.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

