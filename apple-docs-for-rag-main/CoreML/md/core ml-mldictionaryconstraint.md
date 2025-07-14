

- Core ML
-  MLDictionaryConstraint 

Class

# MLDictionaryConstraint

The constraint on the keys for a dictionary feature.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLDictionaryConstraint
```

## Topics

### Accessing the Constraint

var keyType: MLFeatureType

The key type for the dictionary.

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

### Accessing Feature Constraints

var imageConstraint: MLImageConstraint?

The size and format constraints for an image feature.

class MLImageConstraint

The width, height, and pixel format constraints of an image feature.

var dictionaryConstraint: MLDictionaryConstraint?

The constraint for a dictionary feature.

var multiArrayConstraint: MLMultiArrayConstraint?

The constraints on a multidimensional array feature.

class MLMultiArrayConstraint

The shape and data type constraints for a multidimensional array feature.

var sequenceConstraint: MLSequenceConstraint?

The constraints for a sequence feature.

class MLSequenceConstraint

The constraints for a sequence feature.

