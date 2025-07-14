

- Network Extension
- NEFilterProviderConfiguration
-  filterPacketProviderBundleIdentifier 

Instance Property

# filterPacketProviderBundleIdentifier

The bundle identifier of the filter packet provider system extension.

macOS 10.15+

``` source
var filterPacketProviderBundleIdentifier: String? { get set }
```

## Discussion

If this property is `nil`, then the framework uses the bundle identifier of the NEFilterPacketProvider extension in the calling app’s bundle. In this case, make sure the calling app’s bundle contains only one NEFilterPacketProvider, so there’s no ambiguity about which one to use.

This property only applies to system extensions, since macOS doesn’t support implementing a filter packet provider as an app extension.

## See Also

### Accessing bundle identifiers

var filterDataProviderBundleIdentifier: String?

The bundle identifier of the filter data provider system extension.

