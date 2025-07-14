

- Core ML
- MLShapedArrayProtocol
-  init(identityMatrixOfSize:) 

Initializer

# init(identityMatrixOfSize:)

Creates a shaped array type that’s an identity matrix of integers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(identityMatrixOfSize size: Int)
```

Available when `Scalar` conforms to `FixedWidthInteger`.

## Parameters 

`size`  

The size of the identity matrix. For example, a size of `5` creates a 5x5 identity matrix.

## See Also

### Creating a Shaped Array Type

init&lt;S>(scalars: S, shape: [Int])

Creates a shaped array type from an array of values.

init(repeating: Self.Scalar, shape: [Int])

Creates a shaped array type that initializes every element to the same value.

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

