

- Network Extension
- NEDNSProxyManager
-  isEnabled 

Instance Property

# isEnabled

The status of a DNS proxy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

Only one DNS proxy can be active in the system at a time. Therefore, setting this property to true disables any DNS proxy configurations of other apps. Similarly, the system sets this property to false when any other DNS proxy configuration is enabled.

## See Also

### Accessing DNS proxy configuration properties

var providerProtocol: NEDNSProxyProviderProtocol?

The provider-specific portion of the DNS proxy configuration.

var localizedDescription: String?

A description of the DNS proxy.

