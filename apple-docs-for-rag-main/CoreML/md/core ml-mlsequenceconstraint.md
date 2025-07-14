

- Core ML
-  MLSequenceConstraint 

Class

# MLSequenceConstraint

The constraints for a sequence feature.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLSequenceConstraint
```

## Topics

### Accessing the Constraints

var valueDescription: MLFeatureDescription

The description that all sequence elements must match.

var countRange: NSRange

The range of values allowed for the sequence’s length.

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

class MLDictionaryConstraint

The constraint on the keys for a dictionary feature.

var multiArrayConstraint: MLMultiArrayConstraint?

The constraints on a multidimensional array feature.

class MLMultiArrayConstraint

The shape and data type constraints for a multidimensional array feature.

var sequenceConstraint: MLSequenceConstraint?

The constraints for a sequence feature.

