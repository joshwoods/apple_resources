

- Core ML
- MLModelConfiguration
-  parameters 

Instance Property

# parameters

A dictionary of configuration settings your app can override when loading a model.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var parameters: [MLParameterKey : Any]? { get set }
```

## See Also

### Configuring Model Parameters

var modelDisplayName: String?

A human readable name of a model for display purposes.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

