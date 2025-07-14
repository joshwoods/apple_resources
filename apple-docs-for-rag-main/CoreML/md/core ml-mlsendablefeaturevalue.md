

- Core ML
-  MLSendableFeatureValue 

Structure

# MLSendableFeatureValue

A sendable feature value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct MLSendableFeatureValue
```

## Overview

This version of feature value is similar to MLFeatureValue but it can be passed across concurrency domains. Once in the target concurrency domain, you can then convert it to a MLFeatureValue.

## Topics

### Initializers

init([String : Int])

Creates a feature value containing a dictionary of strings to integers.

init(String)

Creates a feature value containing a string value.

init([String : Double])

Creates a feature value containing a dictionary of strings to doubles.

init(Int)

Creates a feature value containing an integer.

init(Double)

Creates a feature value containing a double-precision floating-point value.

init(Float)

Creates a feature value containing a single-precision floating-point value.

init?(MLFeatureValue)

Creates a sendable feature value from a feature value.

init&lt;Scalar>(MLShapedArray&lt;Scalar>)

Creates a feature value containing a shaped array.

init([String])

Creates a feature value containing an array of string values.

init(Int32)

Creates a feature value containing an integer.

init([Int : Double])

Creates a feature value containing a dictionary of integers to doubles.

init([Int : Int])

Creates a feature value containing a dictionary of integers to integers.

init(Float16)

Creates a feature value containing a 16-bit floating-point value.

init(undefined: MLFeatureType)

Creates an undefined feature value of a specific type.

### Instance Properties

var doubleValue: Double?

The double-precision floating-point value, if the contained value is a double.

var float16Value: Float16?

The 16-bit floating-point value, if the contained value is a 16-bit float.

var floatValue: Float?

The single-precision floating-point value, if the contained value is a float.

var integerDictionaryValue: [Int : Double]?

The integer dictionary value, if the contained value is a dictionary of integers to numbers.

var integerValue: Int?

The integer value, if the contained value is an integer.

var isScalar: Bool

A Boolean value indicating whether the value is a single number.

var isShapedArray: Bool

A Boolean value indicating whether the value is a shaped array.

var isUndefined: Bool

A Boolean value indicating whether the value is missing or undefined.

var stringArrayValue: [String]?

The string array value, if the contained value is an array of string.

var stringDictionaryValue: [String : Double]?

The string dictionary value, if the contained value is a dictionary of strings to numbers.

var stringValue: String?

The string value, if the contained value is a string.

var type: MLFeatureType

The type of value.

### Instance Methods

func shapedArrayValue&lt;Scalar>(of: Scalar.Type) -> MLShapedArray&lt;Scalar>?

Returns the shaped array value, if the contained value is a shaped array of the specified type.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Model inputs and outputs

Making Predictions with a Sequence of Inputs

Integrate a recurrent neural network model to process sequences of inputs.

class MLFeatureValue

A generic wrapper around an underlying value and the value’s type.

protocol MLFeatureProvider

An interface that represents a collection of values for either a model’s input or its output.

class MLDictionaryFeatureProvider

A convenience wrapper for the given dictionary of data.

protocol MLBatchProvider

An interface that represents a collection of feature providers.

class MLArrayBatchProvider

A convenience wrapper for batches of feature providers.

class MLModelAsset

An abstraction of a compiled Core ML model asset.

