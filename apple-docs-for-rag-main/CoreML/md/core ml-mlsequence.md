

- Core ML
-  MLSequence 

Class

# MLSequence

A machine learning collection type that stores a series of strings or integers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
class MLSequence
```

## Overview

A sequence stores a series of integers or strings of any length as the underlying type of an `MLFeatureValue`. Some classifier models — typically natural language models, such as an NLTagger — produce an MLSequence feature value from their output features.

## Topics

### Creating a Sequence

convenience init(strings: [String])

Creates a sequence of strings from a string array.

convenience init(int64s: [NSNumber])

Creates a sequence of integers from an array of numbers.

convenience init(empty: MLFeatureType)

Creates an empty sequence of strings or integers.

### Identifying the Sequence’s Element Type

var type: MLFeatureType

The underlying type of the sequence’s elements.

### Retrieving the Sequence’s Values

var stringValues: [String]

An array of strings in the sequence.

var int64Values: [NSNumber]

An array of 64-bit integers in the sequence.

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

### Supporting Types

enum MLFeatureType

The possible types for feature values, input features, and output features.

struct MLShapedArray

A machine learning collection type that stores scalar values in a multidimensional array.

protocol MLShapedArrayProtocol

An interface that defines a shaped array type.

class MLMultiArray

A machine learning collection type that stores numeric values in an array with multiple dimensions.

