

- Network Extension
- NEAppPushManager
-  providerConfiguration 

Instance Property

# providerConfiguration

A dictionary that contains vendor-specific key-value pairs, that you use to configure a provider.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
var providerConfiguration: [String : Any] { get set }
```

## Discussion

The dictionary’s values must only use data types supported by PropertyListSerialization; you can’t use custom types for the values.

The manager passes this dictionary as-is to the NEAppPushProvider when the provider starts.

## See Also

### Inspecting provider properties

var providerBundleIdentifier: String?

A string that contains the bundle identifier of the push provider.

