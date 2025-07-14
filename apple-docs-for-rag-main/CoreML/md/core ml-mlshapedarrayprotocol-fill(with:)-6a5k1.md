

- Core ML
- MLShapedArrayProtocol
-  fill(with:) 

Instance Method

# fill(with:)

Assigns the shaped array’s elements to the elements in a collection, repeatedly, if necessary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func fill(with collection: C) where C : Collection, Self.Scalar == C.Element
```

## Parameters 

`collection`  

A collection of elements.

## Discussion

The shaped array assigns the collection’s elements in first-major order, which is equivalent to row-major order for two-dimensional arrays.

## See Also

### Modifying a Shaped Array Type

func fill(with: Self.Scalar)

Assigns the shaped array’s elements to a value.

func withUnsafeMutableShapedBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Provides read-write access of the shaped array’s underlying memory to a closure.

**Required**

