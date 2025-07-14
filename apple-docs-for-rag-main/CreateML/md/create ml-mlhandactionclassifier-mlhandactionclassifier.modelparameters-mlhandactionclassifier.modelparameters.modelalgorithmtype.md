

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.ModelParameters
-  MLHandActionClassifier.ModelParameters.ModelAlgorithmType 

Enumeration

# MLHandActionClassifier.ModelParameters.ModelAlgorithmType

The hand action classifier training algorithm options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum ModelAlgorithmType
```

## Topics

### Choosing an algorithm type

case gcn

Selects the graph convolutional neural-network algorithm for a hand action classifier.

### Comparing an algorithm type

static func == (MLHandActionClassifier.ModelParameters.ModelAlgorithmType, MLHandActionClassifier.ModelParameters.ModelAlgorithmType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Hashing an algorithm type

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Parameter supporting types

struct VideoAugmentationOptions

Options a hand action classification training session can use to generate additional training data from the videos you provide.

enum ValidationData

A dataset a hand action classifier task uses to validate the model during a training session.

