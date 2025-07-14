

- Core ML
- MLModel
-  modelDescription 

Instance Property

# modelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var modelDescription: MLModelDescription { get }
```

## See Also

### Inspecting a Model

static var availableComputeDevices: [MLComputeDevice]

The list of available compute devices that the model’s prediction methods use.

var configuration: MLModelConfiguration

The configuration of the model set during initialization.

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

