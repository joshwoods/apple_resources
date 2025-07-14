

- Core ML
-  MLModelDescription 

Class

# MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLModelDescription
```

## Topics

### Accessing Feature Descriptions

var inputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of input feature descriptions, which the model keys by the input’s name.

var outputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of output feature descriptions, which the model keys by the output’s name.

class MLFeatureDescription

The name, type, and constraints of an input or output feature.

### Accessing Metadata

var classLabels: [Any]?

An array of labels, which can be either strings or a numbers, for classifier models.

var metadata: [MLModelMetadataKey : Any]

A dictionary of the model’s creation information, such as its description, author, version, and license.

struct MLModelMetadataKey

The set of keys the model uses to store values in its metadata dictionary.

### Accessing Prediction Names

var predictedFeatureName: String?

The name of the primary prediction feature output description.

var predictedProbabilitiesName: String?

The name of the feature output description for all probabilities of a prediction.

### Accessing Update Descriptions

var isUpdatable: Bool

A Boolean value that indicates whether you can update the model with additional training.

var trainingInputDescriptionsByName: [String : MLFeatureDescription]

A dictionary of the training input feature descriptions, which the model keys by the input’s name.

var parameterDescriptionsByKey: [MLParameterKey : MLParameterDescription]

A dictionary of the descriptions for the model’s parameters.

class MLParameterDescription

A description of a model parameter that includes a default value and a constraint, if applicable.

### Instance Properties

var stateDescriptionsByName: [String : MLFeatureDescription]

Description of the state features.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting a Model

static var availableComputeDevices: [MLComputeDevice]

The list of available compute devices that the model’s prediction methods use.

var configuration: MLModelConfiguration

The configuration of the model set during initialization.

var modelDescription: MLModelDescription

Model information you use at runtime during development, which Xcode also displays in its Core ML model editor view.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

class MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

