

- Network Extension
- NEFilterProvider
-  filterConfiguration 

Instance Property

# filterConfiguration

An NEFilterProviderConfiguration object containing the current filter configuration.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var filterConfiguration: NEFilterProviderConfiguration { get }
```

## Discussion

The Filter Provider can observe this property to be notified when the configuration changes, using KVO. See Key-Value Observing Programming Guide.

