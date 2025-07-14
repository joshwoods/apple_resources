

- Network Extension
- NEDNSProxyProviderProtocol
-  providerConfiguration 

Instance Property

# providerConfiguration

A dictionary containing vendor-specific configuration parameters for a proxy provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var providerConfiguration: [String : Any]? { get set }
```

## Discussion

This dictionary is passed as-is through the `options` parameter when the framework starts a DNS proxy by calling the proxy’s startProxy(options:completionHandler:) function.

## See Also

### Accessing the DNS proxy configuration

var providerBundleIdentifier: String?

A string containing the bundle identifier of the proxy provider to be used by this configuration.

