

- Core ML
-  MLShapedArraySlice 

Structure

# MLShapedArraySlice

A multidimensional subset of elements from a shaped array type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct MLShapedArraySlice where Scalar : MLShapedArrayScalar
```

## Topics

### Creating a Shaped Array Slice

init(scalar: Scalar)

Creates a shaped array slice with exactly one value and zero dimensions.

init&lt;S>(scalars: S, shape: [Int])

Initialize with a sequence and the shape.

### Creating a Shaped Array Slice from Another Type

init(MLMultiArray)

Creates a new MLShapedArraySlice using a `MLMultiArray` as a backing storage.

init&lt;S>(concatenating: S, alongAxis: Int)

Merges a sequence of shaped arrays into one shaped array along an axis.

### Creating a Shaped Array Slice with Pointers to Memory

init(unsafeUninitializedShape: [Int], initializingWith: (inout UnsafeMutableBufferPointer&lt;Scalar>, [Int]) throws -> Void) rethrows

Creates a shaped array slice from a shape and a closure that initializes its memory.

### Creating a Shaped Array Slice with Data

init(data: Data, shape: [Int])

Creates a shaped array with a defined data and shape.

init(data: Data, shape: [Int], strides: [Int])

Creates a shaped array with defined data, shape, and strides.

### Encoding and Decoding an Array Slice

init(from: any Decoder) throws

Creates an array slice from the passed decoder.

func encode(to: any Encoder) throws

Encodes the array slice.

### Supporting Types

Shaped Array Slice Collection Operations

Properties and methods a shaped array slice inherits from collection protocols.

### Initializers

init(mutating: CVPixelBuffer, shape: [Int])

Creates a new `MLShapedArraySlice` using a pixel buffer as the backing storage.

### Instance Methods

func changingLayout(to: MLShapedArrayBufferLayout) -> MLShapedArraySlice&lt;Scalar>

Returns a copy with the specified buffer layout.

func expandingShape(at: Int) -> MLShapedArraySlice&lt;Scalar>

Returns a new shaped array with expanded dimensions

func reshaped(to: [Int]) -> MLShapedArraySlice&lt;Scalar>

Returns a new reshaped shaped array.

func squeezingShape() -> MLShapedArraySlice&lt;Scalar>

Returns a new squeezed shaped array.

func transposed() -> MLShapedArraySlice&lt;Scalar>

Returns a new transposed shaped array

func transposed(permutation: [Int]) -> MLShapedArraySlice&lt;Scalar>

Returns a new transposed shaped array using a custom permutation.

func withUnsafeMutableShapedBufferPointer&lt;R>(using: MLShapedArrayBufferLayout, (inout UnsafeMutableBufferPointer&lt;Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Calls the given closure with a pointer to the array’s mutable storage that has a specified buffer layout.

### Default Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
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

associatedtype Scalar : MLShapedArrayScalar

Represents the underlying scalar type of the shaped array type.

**Required**

protocol MLShapedArrayScalar

A type that associates a scalar with a shaped array.

protocol MLShapedArrayRangeExpression

An interface for a range expression, which you typically use with subscripts of shaped array types.

