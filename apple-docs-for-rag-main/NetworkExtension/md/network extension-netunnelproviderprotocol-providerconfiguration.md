

- Network Extension
- NETunnelProviderProtocol
-  providerConfiguration 

Instance Property

# providerConfiguration

A dictionary containing keys and values defined by the Tunnel Provider developer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var providerConfiguration: [String : Any]? { get set }
```

## Discussion

All of the keys and values in this dictionary must conform to the NSSecureCoding and NSCopying protocols.

## See Also

### Accessing the tunnel configuration

var providerBundleIdentifier: String?

A string identifying the specific Tunnel Provider extension that should be used with this configuration.

