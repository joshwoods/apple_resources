

- Core ML
- MLModel
-  configuration 

Instance Property

# configuration

The configuration of the model set during initialization.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var configuration: MLModelConfiguration { get }
```

## See Also

### Inspecting a Model

static var availableComputeDevices: [MLComputeDevice]

The list of available compute devices that the model’s prediction methods use.

var modelDescription: MLModelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

