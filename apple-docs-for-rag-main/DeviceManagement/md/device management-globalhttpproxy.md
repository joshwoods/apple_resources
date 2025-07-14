

- Device Management
-  GlobalHTTPProxy 

Device Management Profile

# GlobalHTTPProxy

The payload you use to configure a global HTTP proxy.

iOS 6.0+iPadOS 6.0+macOS 10.9+tvOS 9.0+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object GlobalHTTPProxy
```

## Properties

`ProxyCaptiveLoginAllowed`

`boolean`

If `true`, allows the device to bypass the proxy server to display the login page for captive networks.

Default: `false`

`ProxyPACFallbackAllowed`

`boolean`

If `true`, allows connecting directly to the destination if the proxy autoconfiguration (PAC) file is unreachable.

Default: `false`

`ProxyPACURL`

`string`

The URL of the PAC file that defines the proxy configuration. Starting in iOS 13 and macOS 10.15, only URLs that begin with `http://` or `https://` are allowed.

`ProxyPassword`

`string`

The password used to authenticate to the proxy server.

`ProxyServer`

`string`

The proxy server’s network address.

`ProxyServerPort`

`integer`

The proxy server’s port number.

`ProxyType`

`string`

The proxy type. For a manual proxy type, the profile contains the proxy server address, including its port, and optionally a user name and password. For an auto proxy type, you can enter a PAC URL.

Default: `Manual`

Possible Values: `Manual, Auto`

`ProxyUsername`

`string`

The user name used to authenticate to the proxy server.

## Discussion

Specify `com.apple.proxy.http.global` as the payload type.

There can only be one payload of this type on the device at any time.

### Profile Availability

|                            |                               |
|----------------------------|-------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS |
| User Channel               | \-                            |
| Allow Manual Install       | iOS, macOS, tvOS              |
| Requires Supervision       | iOS, tvOS                     |
| Requires User Approved MDM | \-                            |
| Allowed in User Enrollment | \-                            |
| Allow Multiple Payloads    | \-                            |

### Profile Example

```

    PayloadContent

            ProxyCaptiveLoginAllowed

            ProxyPassword
            password
            ProxyServer
            10.0.1.42
            ProxyServerPort
            8080
            ProxyType
            Manual
            ProxyUsername
            username
            PayloadIdentifier
            com.example.myglobalhttpproxypayload
            PayloadType
            com.apple.proxy.http.global
            PayloadUUID
            dee0892a-7d4c-41be-ac88-d87247dd076c
            PayloadVersion
            1

    PayloadDisplayName
    GlobalHTTPProxy
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    ee2f890c-6c9f-49be-9e19-b81c66d5cc0d
    PayloadVersion
    1

```

## See Also

### Proxies

object DNSProxy

The payload you use to configure DNS proxies.

object NetworkProxyConfiguration

The payload you use to configure network proxies for a device.

