

- Core ML
- MLModel
-  availableComputeDevices 

Type Property

# availableComputeDevices

The list of available compute devices that the model’s prediction methods use.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var availableComputeDevices: [MLComputeDevice] { get }
```

## See Also

### Inspecting a Model

var configuration: MLModelConfiguration

The configuration of the model set during initialization.

var modelDescription: MLModelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

