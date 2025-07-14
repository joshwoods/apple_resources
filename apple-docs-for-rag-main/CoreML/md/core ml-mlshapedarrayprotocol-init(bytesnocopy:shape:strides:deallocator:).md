

- Core ML
- MLShapedArrayProtocol
-  init(bytesNoCopy:shape:strides:deallocator:) 

Initializer

# init(bytesNoCopy:shape:strides:deallocator:)

Creates a shaped array type from a data pointer with memory strides.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    bytesNoCopy bytes: UnsafeRawPointer,
    shape: [Int],
    strides: [Int],
    deallocator: Data.Deallocator
)
```

**Required**

## Parameters 

`bytes`  

An unsafe raw pointer to the data.

`shape`  

An integer array. Each element represents the size of the shaped array’s corresponding dimension.

`strides`  

An integer array. Each element represents the number of memory locations that span the shaped array’s corresponding dimension.

`deallocator`  

A Data.Deallocator.

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

init(unsafeUninitializedShape: [Int], initializingWith: (inout UnsafeMutableBufferPointer&lt;Self.Scalar>, [Int]) throws -> Void) rethrows

Creates a shaped array type from a shape and a closure that initializes its memory.

**Required**

