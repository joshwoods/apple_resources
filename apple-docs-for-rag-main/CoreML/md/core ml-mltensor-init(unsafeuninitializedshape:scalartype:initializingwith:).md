

- Core ML
- MLTensor
-  init(unsafeUninitializedShape:scalarType:initializingWith:) 

Initializer

# init(unsafeUninitializedShape:scalarType:initializingWith:)

Creates a tensor with the specified shape, then calls the given closure with a buffer covering the tensor’s uninitialized memory.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    unsafeUninitializedShape shape: [Int],
    scalarType: any MLTensorScalar.Type,
    initializingWith initializer: (UnsafeMutableRawBufferPointer) throws -> Void
) rethrows
```

## Parameters 

`shape`  

The dimensions of the tensor.

`scalarType`  

The scalar type.

`initializer`  

A closure which will be called to initialize the underlying memory of the tensor. Scalars expected to be stored contiguously in first-major order.

