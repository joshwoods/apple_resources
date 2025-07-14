

- Core ML
- MLShapedArrayProtocol
-  init(scalars:shape:) 

Initializer

# init(scalars:shape:)

Creates a shaped array type from an array of values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    scalars: S,
    shape: [Int]
) where S : Sequence, Self.Scalar == S.Element
```

## Parameters 

`scalars`  

A sequence of values.

`shape`  

An integer array. Each element represents the size of the shaped array’s corresponding dimension.

## See Also

### Creating a Shaped Array Type

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

