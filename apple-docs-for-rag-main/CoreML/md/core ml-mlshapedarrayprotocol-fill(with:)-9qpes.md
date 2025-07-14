

- Core ML
- MLShapedArrayProtocol
-  fill(with:) 

Instance Method

# fill(with:)

Assigns the shaped array’s elements to a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func fill(with value: Self.Scalar)
```

## Parameters 

`value`  

A scalar value.

## See Also

### Modifying a Shaped Array Type

func fill&lt;C>(with: C)

Assigns the shaped array’s elements to the elements in a collection, repeatedly, if necessary.

func withUnsafeMutableShapedBufferPointer&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Scalar>, [Int], [Int]) throws -> R) rethrows -> R

Provides read-write access of the shaped array’s underlying memory to a closure.

**Required**

