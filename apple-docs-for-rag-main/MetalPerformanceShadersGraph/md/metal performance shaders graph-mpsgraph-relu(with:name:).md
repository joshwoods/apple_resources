

- Metal Performance Shaders Graph
- MPSGraph
-  reLU(with:name:) 

Instance Method

# reLU(with:name:)

Computes the ReLU (rectified linear activation unit) function with the input tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func reLU(
    with tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

The operation is: f(x) = max(x, 0).

