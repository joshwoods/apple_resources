

- Core ML
-  MLMultiArray 

Class

# MLMultiArray

A machine learning collection type that stores numeric values in an array with multiple dimensions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class MLMultiArray
```

## Mentioned in 

Making Predictions with a Sequence of Inputs

## Overview

A multidimensional array, or *multiarray*, is one of the underlying types of an `MLFeatureValue` that stores numeric values in multiple dimensions. All elements in an MLMultiArray instance are one of the same type, and one of the types that MLMultiArrayDataType defines:

MLMultiArrayDataType.int32  
32-bit integer

MLMultiArrayDataType.float16  
16-bit floating point number

MLMultiArrayDataType.float32  
32-bit floating point number (also known as float)

float64  
64-bit floating point number (also known as `double` in Swift or `MLMultiArrayDataTypeDouble` in Objective-C)

Each dimension in a multiarray is typically significant or meaningful. For example, a model could have an input that accepts images as a multiarray of pixels with three dimensions, C x H x W. The first dimension, *C*,\_ \_represents the number of color channels, and the second and third dimensions, *H* and *W*, represent the image’s height and width, respectively. The number of dimensions and size of each dimension define the multiarray’s *shape*.

Note

Some models use a one-dimensional multiarray for an input or output. This type of multiarray is conceptually identical to a conventional array.

The shape property is an integer array that has an element for each dimension in the multiarray. Each element in shape defines the size of the corresponding dimension. To inspect the shape and constraints of a model’s multiarray input or output feature:

1.  Access the model’s modelDescription property.

2.  Find the multiarray input or output feature in the model description’s inputDescriptionsByName or outputDescriptionsByName property, respectively.

3.  Access the feature description’s multiArrayConstraint property.

4.  Inspect the multiarray constraint’s shape and shapeConstraint.

## Topics

### Creating a Multiarray

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of integers.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of floats.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of doubles.

init(shape: [NSNumber], dataType: MLMultiArrayDataType) throws

Creates a multidimensional array with a shape and type.

convenience init&lt;ShapedArray>(ShapedArray)

Creates a multiarray from a shaped array.

init(dataPointer: UnsafeMutableRawPointer, shape: [NSNumber], dataType: MLMultiArrayDataType, strides: [NSNumber], deallocator: ((UnsafeMutableRawPointer) -> Void)?) throws

Creates a multiarray from a data pointer.

convenience init(byConcatenatingMultiArrays: [MLMultiArray], alongAxis: Int, dataType: MLMultiArrayDataType)

Merges an array of multiarrays into one multiarray along an axis.

init(pixelBuffer: CVPixelBuffer, shape: [NSNumber])

Creates a multiarray sharing the surface of a pixel buffer.

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

### Inspecting a Multiarray

var count: Int

The total number of elements in the multiarray.

var dataType: MLMultiArrayDataType

The underlying type of the multiarray.

var shape: [NSNumber]

The multiarray’s multidimensional shape as a number array in which each element’s value is the size of the corresponding dimension.

var strides: [NSNumber]

A number array in which each element is the number of memory locations that span the length of the corresponding dimension.

### Providing buffer access

func withUnsafeBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeBufferPointer&lt;S>) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s storage.

func withUnsafeBytes&lt;R>((UnsafeRawBufferPointer) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s storage.

func withUnsafeMutableBufferPointer&lt;S, R>(ofType: S.Type, (UnsafeMutableBufferPointer&lt;S>, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

func withUnsafeMutableBytes&lt;R>((UnsafeMutableRawBufferPointer, [Int]) throws -> R) rethrows -> R

Calls a given closure with a raw pointer to the multiarray’s mutable storage.

### Accessing a Multiarray’s Elements

subscript(Int) -> NSNumber

Accesses the multiarray by using a linear offset.

subscript([NSNumber]) -> NSNumber

Accesses the multiarray by using a number array that has an element for each dimension.

var pixelBuffer: CVPixelBuffer?

A reference to the multiarray’s underlying pixel buffer.

var dataPointer: UnsafeMutableRawPointer

A pointer to the multiarray’s underlying memory.

Deprecated

### Initializers

convenience init(shape: [Int], dataType: MLMultiArrayDataType, strides: [Int])

Creates the object with specified strides.

### Instance Methods

func transfer(to: MLMultiArray)

Transfer the contents to the destination multi-array.

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

class MLSequence

A machine learning collection type that stores a series of strings or integers.

