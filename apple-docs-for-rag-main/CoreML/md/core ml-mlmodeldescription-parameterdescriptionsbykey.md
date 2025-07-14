

- Core ML
- MLModelDescription
-  parameterDescriptionsByKey 

Instance Property

# parameterDescriptionsByKey

A dictionary of the descriptions for the model’s parameters.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
var parameterDescriptionsByKey: [MLParameterKey : MLParameterDescription] { get }
```

## See Also

### Accessing Update Descriptions

var isUpdatable: Bool

A Boolean value that indicates whether you can update the model with additional training.

var trainingInputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of the training input feature descriptions, which the model keys by the input’s name.

class MLParameterDescription

A description of a model parameter that includes a default value and a constraint, if applicable.

