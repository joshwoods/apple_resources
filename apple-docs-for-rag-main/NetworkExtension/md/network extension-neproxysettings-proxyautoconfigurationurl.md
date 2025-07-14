

- Network Extension
- NEProxySettings
-  proxyAutoConfigurationURL 

Instance Property

# proxyAutoConfigurationURL

A URL specifying the location from where the Proxy Auto Configuration (PAC) script should be downloaded.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var proxyAutoConfigurationURL: URL? { get set }
```

## Discussion

If autoProxyConfigurationEnabled is set to true and proxyAutoConfigurationJavaScript is set to nil then the system will download the PAC script from this location and execute the script to determine what proxies to use (if any) for HTTP and HTTPS connections.

## See Also

### Accessing Automatic Proxy Properties

var autoProxyConfigurationEnabled: Bool

A Boolean indicating if proxy auto-configuration is enabled.

var proxyAutoConfigurationJavaScript: String?

A string containing the Proxy Auto Configuration (PAC) JavaScript source code.

