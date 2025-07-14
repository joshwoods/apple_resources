

- Core ML
- MLShapedArrayProtocol
-  withUnsafeMutableShapedBufferPointer(\_:) 

Instance Method

# withUnsafeMutableShapedBufferPointer(\_:)

Provides read-write access of the shaped array’s underlying memory to a closure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func withUnsafeMutableShapedBufferPointer(_ body: (inout UnsafeMutableBufferPointer, [Int], [Int]) throws -> R) rethrows -> R
```

**Required**

## Parameters 

`body`  

A closure that accesses a shaped array’s underlying memory.

## Discussion

The method returns the value your closure returns, if applicable.

## See Also

### Modifying a Shaped Array Type

func fill(with: Self.Scalar)

Assigns the shaped array’s elements to a value.

func fill&lt;C>(with: C)

Assigns the shaped array’s elements to the elements in a collection, repeatedly, if necessary.

