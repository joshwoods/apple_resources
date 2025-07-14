

- Core ML
-  MLFeatureType 

Enumeration

# MLFeatureType

The possible types for feature values, input features, and output features.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum MLFeatureType
```

## Topics

### Enumeration Cases

case int64

The type for integer features and feature values.

case double

The type for double features and feature values.

case image

The type for image features and feature values.

case multiArray

The type for multidimensional array features and feature values.

case string

The type for string features and feature values.

case dictionary

The type for dictionary features and feature values.

case sequence

The type for sequence features and feature values.

case invalid

The type for invalid feature values.

case state

MLState. Represents a model state that may be updated in each inference.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct MLShapedArray

A machine learning collection type that stores scalar values in a multidimensional array.

protocol MLShapedArrayProtocol

An interface that defines a shaped array type.

class MLMultiArray

A machine learning collection type that stores numeric values in an array with multiple dimensions.

class MLSequence

A machine learning collection type that stores a series of strings or integers.

