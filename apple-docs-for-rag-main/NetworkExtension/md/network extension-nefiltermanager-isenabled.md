

- Network Extension
- NEFilterManager
-  isEnabled 

Instance Property

# isEnabled

A Boolean used to toggle the enabled state of the filter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
var isEnabled: Bool { get set }
```

## Discussion

Setting this property to true and saving the configuration will disable all other network content filters on the system, and will start the filter’s Filter Provider extensions. Setting this property to false and saving the configuration will disable the filter and stop the filter’s Filter Provider extensions.

## See Also

### Accessing filter configuration properties

var providerConfiguration: NEFilterProviderConfiguration?

A NEFilterProviderConfiguration object containing the filter configuration settings.

var localizedDescription: String?

A string containing a description of the filter configuration.

