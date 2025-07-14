

- Metal Performance Shaders Graph
- MPSGraph
-  softMax(with:axis:name:) 

Instance Method

# softMax(with:axis:name:)

Computes the softmax function on the input tensor along the specified axis.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func softMax(
    with tensor: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`axis`  

The axis along which softmax is computed.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

