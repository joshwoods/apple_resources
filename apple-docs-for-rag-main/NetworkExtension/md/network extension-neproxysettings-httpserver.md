

- Network Extension
- NEProxySettings
-  httpServer 

Instance Property

# httpServer

An NEProxyServer object containing the static HTTP proxy server settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying
var httpServer: NEProxyServer? { get set }
```

## Discussion

If autoProxyConfigurationEnabled is false and httpEnabled is true, then the proxy server specified in this property will be used for HTTP connections.

## See Also

### Related Documentation

var autoProxyConfigurationEnabled: Bool

A Boolean indicating if proxy auto-configuration is enabled.

### Accessing Manual Proxy Properties

var httpEnabled: Bool

A Boolean indicating if a static HTTP proxy will be used.

var httpsEnabled: Bool

A Boolean indicating if a static HTTPS proxy will be used.

var httpsServer: NEProxyServer?

An NEProxyServer object containing the static HTTPS proxy server settings.

class NEProxyServer

`NEProxyServer` contains settings for a proxy server.

