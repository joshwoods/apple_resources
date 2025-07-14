

- Core ML
-  MLShapedArrayProtocol 

Protocol

# MLShapedArrayProtocol

An interface that defines a shaped array type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol MLShapedArrayProtocol : ExpressibleByArrayLiteral, MutableCollection, RandomAccessCollection where Self.Index == Int
```

## Topics

### Creating a Shaped Array Type

init&lt;S>(scalars: S, shape: [Int])

Creates a shaped array type from an array of values.

init(repeating: Self.Scalar, shape: [Int])

Creates a shaped array type that initializes every element to the same value.

init(identityMatrixOfSize: Int)

Creates a shaped array type that’s an identity matrix of integers.

init(randomScalarsIn: Range&lt;Self.Scalar>, shape: [Int])

Creates a shaped array type that initializes the elements to random integer values within a range.

init(bytesNoCopy: UnsafeRawPointer, shape: [Int], deallocator: Data.Deallocator)

Creates a shaped array type from a data pointer.

init(bytesNoCopy: UnsafeRawPointer, shape: [Int], strides: [Int], deallocator: Data.Deallocator)

Creates a shaped array type from a data pointer with memory strides.

**Required**

init(unsafeUninitializedShape: [Int], initializingWith: (inout UnsafeMutableBufferPointer&lt;Self.Scalar>, [Int]) throws -> Void) rethrows

Creates a shaped array type from a shape and a closure that initializes its memory.

**Required**

### Creating a Shaped Array Type from Another Type

init(MLMultiArray)

Creates a shaped array type from a multiarray.

init(converting: MLMultiArray)

Creates a shaped array type by converting a multiarray.

init&lt;T>(converting: T)

Creates a shaped array type by converting another shaped array type.

### Inspecting a Shaped Array Type

var shape: [Int]

An integer array in which each element represents the size of the corresponding dimension.

**Required**

var strides: [Int]

An integer array in which each element is the number of memory locations that spans the length of the corresponding dimension.

**Required**

var count: Int

The number of elements in the shaped array’s first dimension.

var isScalar: Bool

A Boolean value that indicates whether the shaped array lacks a shape.

var scalarCount: Int

The total number of elements in the shaped array type.

var scalar: Self.Scalar?

A computed property that returns the first element when the shape isn’t empty, or sets the shaped array’s underlying scalar type.

var scalars: [Self.Scalar]

A computed property that generates a linear array that contains every element, or assigns the elements of an array to the shaped array’s elements.

func withUnsafeShapedBufferPointer&lt;R>((UnsafeBufferPointer&lt;Self.Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Provides read-only access of the shaped array’s underlying memory to a closure.

**Required**

### Accessing Elements

subscript&lt;C>(scalarAt _: C) -> Self.Scalar

Accesses an element and a multidimensional location.

**Required** Default implementation provided.

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

Accesses a slice using a collection of integers, in which each element is an index in the corresponding dimension.

**Required** Default implementations provided.

subscript&lt;C>(C) -> MLShapedArraySlice&lt;Self.Scalar>

Accesses a slice using a collection of integer ranges, in which each element is a range in the corresponding dimension.

**Required** Default implementations provided.

### Modifying a Shaped Array Type

func fill(with: Self.Scalar)

Assigns the shaped array’s elements to a value.

func fill&lt;C>(with: C)

Assigns the shaped array’s elements to the elements in a collection, repeatedly, if necessary.

func withUnsafeMutableShapedBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Provides read-write access of the shaped array’s underlying memory to a closure.

**Required**

### Supporting Types

associatedtype Scalar : MLShapedArrayScalar

Represents the underlying scalar type of the shaped array type.

**Required**

struct MLShapedArraySlice

A multidimensional subset of elements from a shaped array type.

protocol MLShapedArrayScalar

A type that associates a scalar with a shaped array.

protocol MLShapedArrayRangeExpression

An interface for a range expression, which you typically use with subscripts of shaped array types.

### Initializers

init(identityMatrixOfSize: Int)

Initialize as an identity matrix.

init(randomScalarsIn: Range&lt;Self.Scalar>, shape: [Int])

Initialize the shaped array with random scalar values.

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- ExpressibleByArrayLiteral
- MutableCollection
- RandomAccessCollection
- Sequence

### Conforming Types

- MLShapedArray
- MLShapedArraySlice

## See Also

### Supporting Types

enum MLFeatureType

The possible types for feature values, input features, and output features.

struct MLShapedArray

A machine learning collection type that stores scalar values in a multidimensional array.

class MLMultiArray

A machine learning collection type that stores numeric values in an array with multiple dimensions.

class MLSequence

A machine learning collection type that stores a series of strings or integers.

