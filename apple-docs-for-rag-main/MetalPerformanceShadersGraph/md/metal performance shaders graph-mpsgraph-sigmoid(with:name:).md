

- Metal Performance Shaders Graph
- MPSGraph
-  sigmoid(with:name:) 

Instance Method

# sigmoid(with:name:)

Computes the sigmoid operation on an input tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func sigmoid(
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

