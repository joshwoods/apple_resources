

- Device Management
-  NetworkProxyConfiguration 

Device Management Profile

# NetworkProxyConfiguration

The payload you use to configure network proxies for a device.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object NetworkProxyConfiguration
```

## Properties

`Proxies`

NetworkProxyConfiguration.Proxies

 (Required) 

The dictionary containing all the proxies for this device.

## Discussion

Specify `com.apple.SystemConfiguration` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            Proxies

                Exceptions

                    *.local, 169.254/16

                HTTPEnable
                1
                HTTPProxy
                proxy.example.com
                HTTPPort
                8080
                FTPPassive
                1

            PayloadIdentifier
            com.example.myproxypayload
            PayloadType
            com.apple.SystemConfiguration
            PayloadUUID
            db29e77a-58ee-404b-8579-935a202cf16c
            PayloadVersion
            1

    PayloadDisplayName
    Network Proxy Configuration
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b2b00925-6565-4e56-85ab-e012ee0ce4e9
    PayloadVersion
    1

```

## Topics

### Objects

object NetworkProxyConfiguration.Proxies

The payload for configuring network proxies.

## See Also

### Proxies

object DNSProxy

The payload you use to configure DNS proxies.

object GlobalHTTPProxy

The payload you use to configure a global HTTP proxy.

