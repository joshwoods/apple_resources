

- Device Management
-  Cellular 

Device Management Profile

# Cellular

The payload you use to configure cellular settings.

iOS 7.0+iPadOS 7.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object Cellular
```

## Properties

`APNs`

`[`Cellular.APNsItem`]`

An array of access point name (APN) dictionaries.

`AttachAPN`

Cellular.AttachAPN

A configuration dictionary.

## Discussion

Specify `com.apple.cellular` as the payload type.

### Profile Availability

|                            |                           |
|----------------------------|---------------------------|
| Device Channel             | iOS, Shared iPad, watchOS |
| User Channel               | \-                        |
| Allow Manual Install       | iOS, watchOS              |
| Requires Supervision       | \-                        |
| Requires User Approved MDM | \-                        |
| Allowed in User Enrollment | \-                        |
| Allow Multiple Payloads    | \-                        |

### Profile Example

```

    PayloadContent

            AttachAPN

                Name
                example.com

            PayloadIdentifier
            com.example.mycellularnetworkpayload
            PayloadType
            com.apple.cellular
            PayloadUUID
            5a024a67-119f-4b38-8648-4c28a054ec5f
            PayloadVersion
            1

    PayloadDisplayName
    Cellular
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    07eeff13-902a-408b-9bec-2228b86f944f
    PayloadVersion
    1

```

## Topics

### Objects

object Cellular.APNsItem

A dictionary that contains details about an access point name (APN) configuration.

object Cellular.AttachAPN

A dictionary that contains details about an attach access point name (APN) configuration.

## See Also

### Networking

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

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

