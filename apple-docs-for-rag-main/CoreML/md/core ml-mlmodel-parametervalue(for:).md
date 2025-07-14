

- Core ML
- MLModel
-  parameterValue(for:) 

Instance Method

# parameterValue(for:)

Returns a model parameter value for a key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func parameterValue(for key: MLParameterKey) throws -> Any
```

## Parameters 

`key`  

The key to a model parameter value.

## See Also

### Inspecting a Model

static var availableComputeDevices: [MLComputeDevice]

The list of available compute devices that the model’s prediction methods use.

var configuration: MLModelConfiguration

The configuration of the model set during initialization.

var modelDescription: MLModelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

