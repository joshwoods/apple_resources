

- Device Management
-  WiFiManagedSettings 

Device Management Profile

# WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object WiFiManagedSettings
```

## Properties

`RequireAdminForAirPortNetworkChange`

`boolean`

If `true`, requires administrator authorization for network changes.

Default: `false`

`RequireAdminForIBSS`

`boolean`

If `true`, requires administrator authorization to enable IBSS.

Default: `false`

`RequireAdminToTurnAirPortOnOff`

`boolean`

If `true`, requires administrator authorization to turn Wi-Fi on or off.

Default: `false`

## Discussion

Specify `com.apple.MCX` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User-Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            RequireAdminForAirPortNetworkChange

            RequireAdminForIBSS

            RequireAdminToTurnAirPortOnOff

            PayloadIdentifier
            com.example.mymanagedwifipayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            8d527efa-0768-49e4-b328-9b222d23c379
            PayloadVersion
            1

    PayloadDisplayName
    Managed Wi-Fi
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    944429fb-2a8d-4d48-81ab-056428104593
    PayloadVersion
    1

```

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

object WiFi

The payload you use to configure Wi-Fi settings.

