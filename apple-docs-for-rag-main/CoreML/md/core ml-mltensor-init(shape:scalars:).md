

- Core ML
- MLTensor
-  init(shape:scalars:) 

Initializer

# init(shape:scalars:)

Creates a tensor with the specified shape and contiguous scalars in first-major order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    shape: [Int],
    scalars: some Collection
)
```

## Parameters 

`shape`  

The dimensions of the tensor. The product of the dimensions of the shape must equal the number of scalars.

`scalars`  

The scalar contents of the tensor.

