

- Device Management
-  Domains 

Device Management Profile

# Domains

The payload you use to configure the domains under an organization’s management.

iOS 8.0+iPadOS 8.0+macOS 10.10+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object Domains
```

## Properties

`CrossSiteTrackingPreventionRelaxedApps`

`[string]`

`CrossSiteTrackingPreventionRelaxedDomains`

`[string]`

An array of up to 10 strings. URLs matching the patterns listed here have relaxed enforcement of cross-site tracking prevention.

Available in iOS 16.2 and later and macOS 13.1 and later.

`EmailDomains`

`[string]`

An array of domains. The system considers email addresses that lack a suffix matching any of these strings out of domain and marked in Mail.

Available in iOS 8 and later and macOS 10.10 and later.

`SafariPasswordAutoFillDomains`

`[string]`

An array of domains. Users can only save passwords in Safari from URLs matching the patterns listed here. This property doesn’t disable the autofill feature itself.

Supervised devices or Shared iPads need this property to enable saving passwords in Safari.

Available in iOS 9.3 and later.

`WebDomains`

`[string]`

An array of domains. The system considers URLs matching the patterns listed in this property managed.

Available in iOS 9.3 and later.

## Discussion

Specify `com.apple.domains` as the payload type.

A URL that begins with the prefix `www.` is treated as though it doesn’t contain that prefix during matching. For example, `http://www.apple.com/store` is matched as `http://apple.com/store`.

Trailing slashes are ignored.

If a domain string entry contains a port number, the system considers only addresses that specify that port number managed. Otherwise, the system matches the domain without regard to the port number specified. For example, the pattern `*.apple.com:8080` matches `http://site.apple.com:8080/page.html` but not `http://site.apple.com/page.html`, while the pattern `*.apple.com` matches both URLs.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | \-                      |
| Allow Multiple Payloads    | \-                      |

### Profile Example

```

    PayloadContent

            EmailDomains

                example.com

            SafariPasswordAutoFillDomains

                example.com

            WebDomains

                example.com

            PayloadIdentifier
            com.example.mysafaridomainspayload
            PayloadType
            com.apple.domains
            PayloadUUID
            0f94e664-4c36-4637-b264-19a533adc8e1
            PayloadVersion
            1

    PayloadDisplayName
    Domains
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    0cf6d95f-8e9f-49f3-9cba-c5e78de5430e
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

