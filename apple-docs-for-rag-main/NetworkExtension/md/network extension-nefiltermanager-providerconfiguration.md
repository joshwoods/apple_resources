

- Network Extension
- NEFilterManager
-  providerConfiguration 

Instance Property

# providerConfiguration

A NEFilterProviderConfiguration object containing the filter configuration settings.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var providerConfiguration: NEFilterProviderConfiguration? { get set }
```

## Discussion

If this property is nil after calling `loadFromPreferencesWithCompletionHandler:`, then the filter configuration does not exist in the Network Extension preferences.

## See Also

### Accessing filter configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the filter.

var localizedDescription: String?

A string containing a description of the filter configuration.

