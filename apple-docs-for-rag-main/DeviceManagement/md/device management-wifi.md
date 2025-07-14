

- Device Management
-  WiFi 

Device Management Profile

# WiFi

The payload you use to configure Wi-Fi settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object WiFi
```

## Properties

`AutoJoin`

`boolean`

If `true`, the device joins the network automatically.

If `false`, the user must tap the network name to join it.

Available in iOS 5.0 and later, and in macOS 10.7 and later.

Default: `true`

`CaptiveBypass`

`boolean`

If `true`, the system bypasses Captive Network detection when the device connects to the network. Available in iOS 10.0 and later.

Default: `false`

`DisableAssociationMACRandomization`

`boolean`

If `true,` disables MAC address randomization for a Wi-Fi network while associated with that network. This feature also shows a privacy warning in Settings indicating that the network has reduced privacy protections.

If `false`, then the system enables MAC address randomization.

This value is only locked when MDM installs the profile. If the profile is manually installed, the system sets the value but the user can change it. Available in iOS 14 and later, macOS 15 and later, and watchOS 7 and later.

Default: `false`

`DisplayedOperatorName`

`string`

The operator name to display when connected to this network. Used only with Wi-Fi Hotspot 2.0 access points. Available in iOS 7.0 and later, and in macOS 10.9 and later.

`DomainName`

`string`

The primary domain of the tunnel. Available in iOS 7.0 and later, and in macOS 10.9 and later.

`EAPClientConfiguration`

WiFi.EAPClientConfiguration

The enterprise network configuration.

`EnableIPv6`

`boolean`

If `true`, enables IPv6 on this interface.

Default: `true`

`EncryptionType`

`string`

The encryption type for the network.

If set to anything except `None`, the payload may contain the following three keys: `Password`, `PayloadCertificateUUID`, or `EAPClientConfiguration`.

As of iOS 16, tvOS 16, watchOS 9, and macOS 13:

- `WPA` allows joining WPA or WPA2 networks

- `WPA2` allows joining WPA2 or WPA3 networks

- `WPA3` allows joining WPA3 networks only

- `Any` allows joining WPA, WPA2, WPA3, and WEP networks

Prior to iOS 16, tvOS 16, and watchOS 9, specifying `WPA`, `WPA2`, and `WPA3` were equivalent and would allow joining any WPA network.

Prior to macOS 13, the encryption type, if specified explicitly, needed to match the encryption type of the network exactly.

Default: `Any`

Possible Values: `WEP, WPA, WPA2, WPA3, Any, None`

`HESSID`

`string`

The HESSID used for Wi-Fi Hotspot 2.0 negotiation.

`HIDDEN_NETWORK`

`boolean`

If `true`, defines this network as hidden.

Default: `false`

`IsHotspot`

`boolean`

If `true`, the device treats the network as a hotspot. Available in iOS 7.0 and later, and in macOS 10.9 and later.

Default: `false`

`MCCAndMNCs`

`[string]`

An array of Mobile Country Code/Mobile Network Code (MCC/MNC) pairs used for Wi-Fi Hotspot 2.0 negotiation. Each string must contain exactly six digits. Available in iOS 7.0 and later. This feature isn’t supported in macOS.

`NAIRealmNames`

`[string]`

An array of Network Access Identifier Realm names used for Wi-Fi Hotspot 2.0 negotiation. Available in iOS 7.0 and later, and in macOS 10.9 and later.

`Password`

`string`

The password for the access point.

`PayloadCertificateUUID`

`string`

The UUID of the certificate payload within the same profile to use for the client credential.

`ProxyPACFallbackAllowed`

`boolean`

If `true`, allows connecting directly to the destination if the PAC file is unreachable.

Default: `false`

`ProxyPACURL`

`string`

The URL of the PAC file that defines the proxy configuration.

`ProxyPassword`

`string`

The password used to authenticate to the proxy server.

`ProxyServer`

`string`

The proxy server’s network address.

`ProxyServerPort`

`integer`

The proxy server’s port number.

Minimum: `0`

Maximum: `65535`

`ProxyType`

`string`

The proxy type, if any, to use. If you choose the manual proxy type, you need the proxy server address, including its port and optionally a user name and password into the proxy server. If you choose the auto proxy type, you can enter a proxy autoconfiguration (PAC) URL. Available in iOS 5.0 and later, and on all versions of macOS.

Default: `None`

Possible Values: `None, Manual, Auto`

`ProxyUsername`

`string`

The user name used to authenticate to the proxy server.

`QoSMarkingPolicy`

WiFi.QoSMarkingPolicy

A dictionary that contains the list of apps that the system allows to benefit from L2 and L3 marking. When this dictionary isn’t present, the system allows all apps to use L2 and L3 marking when the Wi-Fi network supports Cisco QoS fast lane. Available in iOS 10.0 and later, and in macOS 10.13 and later.

`RoamingConsortiumOIs`

`[string]`

An array of Roaming Consortium Organization Identifiers used for Wi-Fi Hotspot 2.0 negotiation. Available in iOS 7.0 and later, and in macOS 10.9 and later.

`ServiceProviderRoamingEnabled`

`boolean`

If `true`, allows connection to roaming service providers. Available in iOS 7.0 and later, and in macOS 10.9 and later.

Default: `false`

`SetupModes`

`[string]`

An array of strings that contain the type of connection mode to attach.

Possible Values: `System, Loginwindow`

`SSID_STR`

`string`

The SSID of the Wi-Fi network to use. In iOS 7.0 and later, the SSID is optional if a value exists for `DomainName` value.

`TLSCertificateRequired`

`boolean`

If `true`, allows for two-factor authentication for EAP-TTLS, PEAP, or EAP-FAST. If `false`, allows for zero-factor authentication for EAP-TLS.

Default: `false`

## Discussion

Specify `com.apple.wifi.managed` as the payload type.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Profile Example

```

    New item

        PayloadContent

                AutoJoin

                CaptiveBypass

                DisableAssociationMACRandomization

                EncryptionType
                WPA
                HIDDEN_NETWORK

                IsHotspot

                Password
                Password123
                PayloadDisplayName
                Wi-Fi
                ProxyType
                None
                SSID_STR
                Example
                PayloadIdentifier
                com.example.mywifipayload
                PayloadType
                com.apple.wifi.managed
                PayloadUUID
                94c487e0-d6f8-41e3-b66d-a89994e6919b
                PayloadVersion
                1

        PayloadDisplayName
        Wi-Fi
        PayloadIdentifier
        com.example.myprofile
        PayloadType
        Configuration
        PayloadUUID
        71e9b0f7-02f8-4aea-b365-b381d872909a
        PayloadVersion
        1

```

## Topics

### Objects

object WiFi.EAPClientConfiguration

A dictionary that configures an enterprise network.

object WiFi.QoSMarkingPolicy

A dictionary that defines the quality-of-service settings.

## See Also

### Networking

object Cellular

The payload you use to configure cellular settings.

object CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

object ContentCaching

The payload you use to configure the content-caching service.

object DNSSettings

The payload you use to configure encrypted DNS settings.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

