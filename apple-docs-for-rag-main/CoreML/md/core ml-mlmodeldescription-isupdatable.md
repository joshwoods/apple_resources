

- Core ML
- MLModelDescription
-  isUpdatable 

Instance Property

# isUpdatable

A Boolean value that indicates whether you can update the model with additional training.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
var isUpdatable: Bool { get }
```

## See Also

### Accessing Update Descriptions

var trainingInputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of the training input feature descriptions, which the model keys by the input’s name.

var parameterDescriptionsByKey: [MLParameterKey : MLParameterDescription]

A dictionary of the descriptions for the model’s parameters.

class MLParameterDescription

A description of a model parameter that includes a default value and a constraint, if applicable.

