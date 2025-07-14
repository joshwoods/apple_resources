

- Core ML
- MLModelDescription
-  inputDescriptionsByName 

Instance Property

# inputDescriptionsByName

A dictionary of input feature descriptions, which the model keys by the input’s name.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var inputDescriptionsByName: [String : MLFeatureDescription] { get }
```

## See Also

### Accessing Feature Descriptions

var outputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of output feature descriptions, which the model keys by the output’s name.

class MLFeatureDescription

The name, type, and constraints of an input or output feature.

