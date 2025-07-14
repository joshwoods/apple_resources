

- Network Extension
- NEProxySettings
-  proxyAutoConfigurationJavaScript 

Instance Property

# proxyAutoConfigurationJavaScript

A string containing the Proxy Auto Configuration (PAC) JavaScript source code.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var proxyAutoConfigurationJavaScript: String? { get set }
```

## Discussion

If autoProxyConfigurationEnabled is set to true then the system will execute the PAC script to determine what proxies to use (if any) for HTTP and HTTPS connections.

## See Also

### Accessing Automatic Proxy Properties

var autoProxyConfigurationEnabled: Bool

A Boolean indicating if proxy auto-configuration is enabled.

var proxyAutoConfigurationURL: URL?

A URL specifying the location from where the Proxy Auto Configuration (PAC) script should be downloaded.

