

- Network Extension
- NETunnelNetworkSettings
-  dnsSettings 

Instance Property

# dnsSettings

The tunnel DNS settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var dnsSettings: NEDNSSettings? { get set }
```

## Discussion

Network connections to hosts in the tunnel’s internal network will use these DNS settings when resolving host names.

## See Also

### Accessing tunnel network settings

var tunnelRemoteAddress: String

The IP address of the tunnel server.

class NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

var proxySettings: NEProxySettings?

The tunnel HTTP proxy settings.

class NEProxySettings

`NEProxySettings` contains HTTP proxy settings.

