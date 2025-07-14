

- Core ML
- MLShapedArrayProtocol
-  strides 

Instance Property

# strides

An integer array in which each element is the number of memory locations that spans the length of the corresponding dimension.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var strides: [Int] { get }
```

**Required**

## See Also

### Inspecting a Shaped Array Type

var shape: [Int]

An integer array in which each element represents the size of the corresponding dimension.

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

