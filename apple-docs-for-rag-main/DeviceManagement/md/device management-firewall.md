

- Device Management
-  Firewall 

Device Management Profile

# Firewall

The payload you use to configure the firewall.

macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object Firewall
```

## Properties

`AllowSigned`

`boolean`

If `true`, the system allows built-in software to receive incoming connections. Available in macOS 12.3 and later.

Note

The system ensures that `AllowSigned` always has a value. If missing from the payload, the system sets it to `true`.

Default: `true`

`AllowSignedApp`

`boolean`

If `true`, the system allows downloaded signed software to receive incoming connections. Available in macOS 12.3 and later.

Note

The system ensures that `AllowSignedApp` always has a value. If missing from the payload, the system sets it to `true`.

Default: `true`

`Applications`

`[`Firewall.ApplicationsItem`]`

The list of apps with connections that the firewall controls.

`BlockAllIncoming`

`boolean`

If `true`, the system enables blocking all incoming connections.

`EnableFirewall`

`boolean`

 (Required) 

If `true`, the system enables the firewall.

`EnableLogging`

`boolean`

Deprecated 

If `true`, the system enables logging. Available in macOS 12 through macOS 14.6.

`EnableStealthMode`

`boolean`

If `true`, the system enables stealth mode.

`LoggingOption`

`string`

Deprecated 

The type of logging. Available in macOS 12 and through macOS 14.6.

Possible Values: `throttled, brief, detail`

## Discussion

Specify `com.apple.security.firewall` as the payload type.

The payload needs to exist in a system-scoped profile.

If more than one profile contains this payload, the system uses the most restrictive union of settings.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            EnableFirewall

            Applications

                    BundleID
                    com.example.myapp
                    Allowed

            PayloadIdentifier
            com.example.myfirewallpayload
            PayloadType
            com.apple.security.firewall
            PayloadUUID
            28b1fef7-ddb6-4d56-9a6a-6bb4e56e7f0b
            PayloadVersion
            1

    PayloadDisplayName
    Firewall
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8f2fa915-f2da-4034-9424-2218355a6f3c
    PayloadVersion
    1

```

## Topics

### Objects

object Firewall.ApplicationsItem

A dictionary of details for apps.

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

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

