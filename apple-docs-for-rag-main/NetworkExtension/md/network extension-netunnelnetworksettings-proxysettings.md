

- Network Extension
- NETunnelNetworkSettings
-  proxySettings 

Instance Property

# proxySettings

The tunnel HTTP proxy settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var proxySettings: NEProxySettings? { get set }
```

## Discussion

HTTP connections to hosts in the tunnel’s internal network will use these proxy settings.

## See Also

### Accessing tunnel network settings

var tunnelRemoteAddress: String

The IP address of the tunnel server.

var dnsSettings: NEDNSSettings?

The tunnel DNS settings.

class NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

class NEProxySettings

`NEProxySettings` contains HTTP proxy settings.

