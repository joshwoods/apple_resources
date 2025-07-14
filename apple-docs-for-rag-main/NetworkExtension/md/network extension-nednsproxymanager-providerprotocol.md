

- Network Extension
- NEDNSProxyManager
-  providerProtocol 

Instance Property

# providerProtocol

The provider-specific portion of the DNS proxy configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var providerProtocol: NEDNSProxyProviderProtocol? { get set }
```

## Discussion

As the author of the DNS proxy, you decide what configuration the proxy needs. For example, if your proxy requires the IP addresses of servers to which DNS traffic can be redirected, you can use an array of strings to hold these values.

Initially, you store this array in the configuration profile, as described in Configuration Profile Reference. When you want to inspect or modify this data, you call loadFromPreferences(completionHandler:) to pull the configuration into memory. You access this memory through the proxy manager’s providerProtocol property.

## See Also

### Accessing DNS proxy configuration properties

var isEnabled: Bool

The status of a DNS proxy.

var localizedDescription: String?

A description of the DNS proxy.

