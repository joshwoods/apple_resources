

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
-  MLActionClassifier.ModelParameters.ModelAlgorithmType 

Enumeration

# MLActionClassifier.ModelParameters.ModelAlgorithmType

The action classifier training algorithm options.

macOS 11.0+

``` source
enum ModelAlgorithmType
```

## Topics

### Designating an algorithm

case stgcn

The spatial-temporal graph convolution neural-network algorithm.

### Hashing an algorithm type

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Comparing algorithm types

static func == (MLActionClassifier.ModelParameters.ModelAlgorithmType, MLActionClassifier.ModelParameters.ModelAlgorithmType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Supporting types

enum ValidationData

The source of a validation dataset for an action classifier.

struct VideoAugmentationOptions

The video augmentations for an action classifier training session.

