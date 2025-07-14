

- Device Management
-  NetworkUsageRules 

Device Management Profile

# NetworkUsageRules

The payload you use to configure network-usage rules.

iOS 9.0+iPadOS 9.0+Device Assignment ServicesVPP License Management

``` source
object NetworkUsageRules
```

## Properties

`ApplicationRules`

`[`NetworkUsageRules.ApplicationRulesItem`]`

An array of application rules, that apply to only managed apps.

`SIMRules`

`[`NetworkUsageRules.SIMRulesItem`]`

An array of SIM rules, that apply to all apps.

## Discussion

Specify `com.apple.networkusagerules` as the payload type.

Network usage rules allow enterprises to specify how devices use networks, such as cellular data networks. iOS 9-12 require the application rules. In iOS 13, application rules, SIM rules, or both must be present.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Allow Manual Install       | \-               |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | \-               |
| Allow Multiple Payloads    | \-               |

### Profile Example

```

    PayloadContent

            ApplicationRules

                    AllowCellularData

                    AllowRoamingCellularData

                    AppIdentifierMatches

                        com.apple.appname

            PayloadIdentifier
            com.example.mynetworkusagepayload
            PayloadType
            com.apple.networkusagerules
            PayloadUUID
            'ef0250de-bfd4-4095-9ad3-34cf1281d5da
            PayloadVersion
            1

    PayloadDisplayName
    Network Usage
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b724f950-5853-4b78-8f4a-9a37a0ccac1f
    PayloadVersion
    1

```

## Topics

### Objects

object NetworkUsageRules.ApplicationRulesItem

The application rules dictionary.

object NetworkUsageRules.SIMRulesItem

The policy for individual SIM cards.

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

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

