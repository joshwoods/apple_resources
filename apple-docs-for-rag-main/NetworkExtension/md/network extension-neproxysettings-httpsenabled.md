

- Network Extension
- NEProxySettings
-  httpsEnabled 

Instance Property

# httpsEnabled

A Boolean indicating if a static HTTPS proxy will be used.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var httpsEnabled: Bool { get set }
```

## See Also

### Accessing Manual Proxy Properties

var httpEnabled: Bool

A Boolean indicating if a static HTTP proxy will be used.

var httpServer: NEProxyServer?

An NEProxyServer object containing the static HTTP proxy server settings.

var httpsServer: NEProxyServer?

An NEProxyServer object containing the static HTTPS proxy server settings.

class NEProxyServer

`NEProxyServer` contains settings for a proxy server.

