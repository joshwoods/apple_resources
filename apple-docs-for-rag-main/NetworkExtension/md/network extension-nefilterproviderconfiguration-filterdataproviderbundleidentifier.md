

- Network Extension
- NEFilterProviderConfiguration
-  filterDataProviderBundleIdentifier 

Instance Property

# filterDataProviderBundleIdentifier

The bundle identifier of the filter data provider system extension.

macOS 10.15+

``` source
var filterDataProviderBundleIdentifier: String? { get set }
```

## Discussion

If this property is `nil`, then the framework uses the bundle identifier of the NEFilterDataProvider extension in the calling app’s bundle. In this case, make sure the calling app’s bundle contains only one NEFilterDataProvider, so there’s no ambiguity about which one to use.

This property only applies to system extensions, since macOS doesn’t support implementing a filter data provider as an app extension.

## See Also

### Accessing bundle identifiers

var filterPacketProviderBundleIdentifier: String?

The bundle identifier of the filter packet provider system extension.

