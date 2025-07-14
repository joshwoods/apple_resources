

- Core ML
-  MLShapedArray 

Structure

# MLShapedArray

A machine learning collection type that stores scalar values in a multidimensional array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MLShapedArray where Scalar : MLShapedArrayScalar
```

## Overview

A shaped array is a multidimensional array type that’s the Swift counterpart to MLMultiArray. MLShapedArray is one of the underlying types of `MLFeatureValue` that stores scalar values. You can convert a shaped array to an MLMultiArray with its init(_:) initializer, and convert back to a shaped array with its init(_:) initializer. All elements in an MLShapedArray are of the same type, and that type must conform to MLShapedArrayScalar:

- Int32

- Float

- Double

Each dimension in a shaped array is typically significant or meaningful. For example, a model could have an input that accepts images as a three-dimensional array of pixels, C x H x W. The first dimension, *C*,\_ \_represents the number of color channels, and the second and third dimensions, *H* and *W*, represent the image’s height and width, respectively. The number of dimensions and size of each dimension define the shaped array’s *shape*.

Note

Some models use a one-dimensional multiarray for an input or output. This type of shaped array is conceptually identical to a conventional Array.

A shaped array’s shape property is an integer array in which each element defines the size of the corresponding dimension. To inspect the shape and constraints of a model’s multiarray input or output feature:

1.  Access the model’s modelDescription property.

2.  Find the multiarray input or output feature in the model description’s inputDescriptionsByName or outputDescriptionsByName property, respectively.

3.  Access the feature description’s multiArrayConstraint property.

4.  Inspect the multiarray constraint’s shape and shapeConstraint.

## Topics

### Creating a Shaped Array

init(scalar: Scalar)

Creates a shaped array with exactly one value and zero dimensions.

init&lt;S>(scalars: S, shape: [Int])

Initialize with a sequence and the shape.

### Creating a Shaped Array from Another Type

init(MLMultiArray)

init&lt;S>(concatenating: S, alongAxis: Int)

Merges a sequence of shaped arrays into one shaped array along an axis.

### Creating a shaped array with pointers to memory

init(unsafeUninitializedShape: [Int], initializingWith: (inout UnsafeMutableBufferPointer&lt;Scalar>, [Int]) throws -> Void) rethrows

Creates a shaped array from a shape and a closure that initializes its memory.

### Creating a shaped array from data

init(data: Data, shape: [Int])

Creates a shaped array from a block of data and a shape.

init(data: Data, shape: [Int], strides: [Int])

Creates a shaped array from a block of data, a shape, and strides.

### Encoding and decoding

init(from: any Decoder) throws

Creates a shaped array from a decoder.

func encode(to: any Encoder) throws

Encode a shaped array.

### Inspecting a Shaped Array

var description: String

A text representation of the shaped array.

### Supporting Types

Shaped Array Collection Operations

Properties and methods a shaped array inherits from collection protocols.

### Initializers

init(mutating: CVPixelBuffer, shape: [Int])

Creates a new `MLShapedArray` using a pixel buffer as the backing storage.

### Instance Methods

func changingLayout(to: MLShapedArrayBufferLayout) -> MLShapedArray&lt;Scalar>

Returns a copy with the specified buffer layout.

func expandingShape(at: Int) -> MLShapedArray&lt;Scalar>

Returns a new shaped array with expanded dimensions.

func reshaped(to: [Int]) -> MLShapedArray&lt;Scalar>

Returns a new reshaped shaped array.

func squeezingShape() -> MLShapedArray&lt;Scalar>

Returns a new squeezed shaped array.

func transposed() -> MLShapedArray&lt;Scalar>

Returns a new transposed shaped array.

func transposed(permutation: [Int]) -> MLShapedArray&lt;Scalar>

Returns a transposed shaped array using a custom permutation.

func withMutablePixelBufferIfAvailable&lt;R>((CVPixelBuffer) throws -> R) rethrows -> R?

Writes to the underlying pixel buffer.

func withPixelBufferIfAvailable&lt;R>((CVPixelBuffer) throws -> R) rethrows -> R?

Reads the underlying pixel buffer.

func withUnsafeMutableShapedBufferPointer&lt;R>(using: MLShapedArrayBufferLayout, (inout UnsafeMutableBufferPointer&lt;Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Calls the given closure with a pointer to the array’s mutable storage that has a specified buffer layout.

### Default Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- MLShapedArrayProtocol
- MutableCollection
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Supporting Types

enum MLFeatureType

The possible types for feature values, input features, and output features.

protocol MLShapedArrayProtocol

An interface that defines a shaped array type.

class MLMultiArray

A machine learning collection type that stores numeric values in an array with multiple dimensions.

class MLSequence

A machine learning collection type that stores a series of strings or integers.

