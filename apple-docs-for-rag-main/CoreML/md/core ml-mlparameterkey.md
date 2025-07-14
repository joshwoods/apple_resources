

- Core ML
-  MLParameterKey 

Class

# MLParameterKey

The keys for the parameter dictionary in a model configuration or a model update context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLParameterKey
```

## Overview

Use an MLParameterKey to retrieve a model’s parameter value using:

- The model’s parameterValue(for:) method

- The parameters dictionary of an MLModelConfiguration

- The parameters dictionary of an MLUpdateContext

Note

To access the parameter of a specific model within a pipeline model, use the parameter key’s scoped(to:) method with the model’s name.

### Overriding Model and Layer Parameters

To override a model’s default parameter values:

1.  Create an MLModelConfiguration instance.

2.  Use an MLParameterKey for each parameter to set its value in the model configuration’s parameters dictionary.

3.  Create a new model instance using init(contentsOf:configuration:) with your custom model configuration.

### Configuring Update Parameters

To configure the update parameters for an MLUpdateTask:

1.  Create an MLModelConfiguration instance.

2.  Use an MLParameterKey for each parameter to set its value in the model configuration’s parameters dictionary.

3.  Create a new update task with your custom model configuration.

See Personalizing a Model with On-Device Updates.

## Topics

### Scoping Parameter Keys

func scoped(to: String) -> MLParameterKey

Creates a copy of a parameter key and adds the scope to it.

### Accessing Model Parameters

class var numberOfNeighbors: MLParameterKey

The key you use to access the number of neighbors that adjusts the affinity of a k-nearest-neighbor model.

class var linkedModelFileName: MLParameterKey

The key you use to access the linked model’s filename.

class var linkedModelSearchPath: MLParameterKey

The key you use to access the linked model’s search path.

### Accessing Neural Network Layer Parameters

class var weights: MLParameterKey

The key you use to access the weights of a layer in a neural network model.

class var biases: MLParameterKey

The key you use to access the biases of a layer in a neural network model.

### Accessing Model Update Parameters

class var learningRate: MLParameterKey

The key you use to access the optimizer’s learning rate parameter.

class var momentum: MLParameterKey

The key you use to access the stochastic gradient descent (SGD) optimizer’s momentum parameter.

class var miniBatchSize: MLParameterKey

The key you use to access the optimizer’s mini batch-size parameter.

class var beta1: MLParameterKey

The key you use to access the Adam optimizer’s first beta parameter.

class var beta2: MLParameterKey

The key you use to access the Adam optimizer’s second beta parameter.

class var eps: MLParameterKey

The key you use to access the Adam optimizer’s epsilon parameter.

class var epochs: MLParameterKey

The key you use to access the optimizer’s epochs parameter.

class var shuffle: MLParameterKey

The key you use to access the shuffle parameter, a Boolean value that determines whether the model randomizes the data between epochs.

class var seed: MLParameterKey

The key you use to access the seed parameter that initializes the random number generator for the shuffle option.

## Relationships

### Inherits From

- MLKey

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
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

class MLModelDescription

Information about a model, primarily the input and output format for each feature the model expects, and optional metadata.

func parameterValue(for: MLParameterKey) throws -> Any

Returns a model parameter value for a key.

