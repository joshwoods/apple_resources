

- Core ML
- MLShapedArrayProtocol
-  init(unsafeUninitializedShape:initializingWith:) 

Initializer

# init(unsafeUninitializedShape:initializingWith:)

Creates a shaped array type from a shape and a closure that initializes its memory.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    unsafeUninitializedShape shape: [Int],
    initializingWith initializer: (inout UnsafeMutableBufferPointer, [Int]) throws -> Void
) rethrows
```

**Required**

## Parameters 

`shape`  

An integer array. Each element represents the size of the shaped array’s corresponding dimension.

`initializer`  

A closure you provide that initializes the shaped array’s underlying memory. The initializer calls your closure with a pointer to the memory and an array of strides that correspond to the shaped array’s dimensions.

## See Also

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

