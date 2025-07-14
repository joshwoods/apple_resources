

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
-  MLSoundClassifier.ModelParameters.FeaturePrintType 

Enumeration

# MLSoundClassifier.ModelParameters.FeaturePrintType

The type options for an Audio Feature Print feature extractor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum FeaturePrintType
```

## Topics

### Designating a feature-print type

case sound

Creates a feature print type for a sound classifier.

### Describing a feature-print type

var description: String

A text representation of the feature-print type.

### Comparing feature-print types

static func == (MLSoundClassifier.ModelParameters.FeaturePrintType, MLSoundClassifier.ModelParameters.FeaturePrintType) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Hashing a feature-print type

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Designating a feature extractor

case audioFeaturePrint(type: MLSoundClassifier.ModelParameters.FeaturePrintType, revision: Int)

Represents the Audio Feature Print extractor.

case vggish(revision: Int)

Represents the VGGish feature extractor, which is compatible with older OS versions.

