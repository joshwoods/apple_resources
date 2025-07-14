

- Network Extension
- NEFilterManager
-  localizedDescription 

Instance Property

# localizedDescription

A string containing a description of the filter configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var localizedDescription: String? { get set }
```

## Discussion

If this property is set to nil at the time that the configuration is created, it will be automatically set to the display name of the calling app.

## See Also

### Accessing filter configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the filter.

var providerConfiguration: NEFilterProviderConfiguration?

A NEFilterProviderConfiguration object containing the filter configuration settings.

