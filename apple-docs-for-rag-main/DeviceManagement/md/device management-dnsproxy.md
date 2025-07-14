

- Device Management
-  DNSProxy 

Device Management Profile

# DNSProxy

The payload you use to configure DNS proxies.

iOS 11.0+iPadOS 11.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object DNSProxy
```

## Properties

`AppBundleIdentifier`

`string`

 (Required) 

The bundle identifier of the app containing the DNS proxy network extension.

`DNSProxyUUID`

`string`

A globally-unique identifier for this DNS proxy configuration. Managed apps with the same `DNSProxyUUID` in their app attributes have their DNS lookups traffic processed by the proxy.

`ProviderBundleIdentifier`

`string`

The bundle identifier of the DNS proxy network extension to use. Declaring the bundle identifier is useful for apps that contain more than one DNS proxy extension.

`ProviderConfiguration`

DNSProxy.ProviderConfiguration

The dictionary of vendor-specific configuration items.

## Discussion

Specify `com.apple.dnsProxy.managed` as the payload type.

Beginning with iOS 15, this profile is unsupervised and needs to be installed through MDM.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | \-                      |
| Allow Manual Install       | macOS                   |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS                     |
| Allow Multiple Payloads    | \-                      |

### Profile Example

```

    PayloadContent

            AppBundleIdentifier
            com.example.mydnsproxyapp
            ProviderBundleIdentifier
            com.example.mydnsproxyapp.mydnsproxyprovider
            ProviderConfiguration

                resolver

                    ipaddress
                    9.9.9.9

            PayloadIdentifier
            com.example.mydnsproxypayload
            PayloadType
            com.apple.dnsProxy.managed
            PayloadUUID
            D6B3F3E4-A72E-49F1-AE2E-742A3A11BE1D
            PayloadVersion
            1

    PayloadDisplayName
    DNS Proxy
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    6a60bbe0-242c-493d-b338-c5885107f2af
    PayloadVersion
    1

```

## Topics

### Objects

object DNSProxy.ProviderConfiguration

The dictionary of vendor-specific configuration items.

## See Also

### Proxies

object GlobalHTTPProxy

The payload you use to configure a global HTTP proxy.

object NetworkProxyConfiguration

The payload you use to configure network proxies for a device.

