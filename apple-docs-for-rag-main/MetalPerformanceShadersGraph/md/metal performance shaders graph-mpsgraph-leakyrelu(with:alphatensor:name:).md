

- Metal Performance Shaders Graph
- MPSGraph
-  leakyReLU(with:alphaTensor:name:) 

Instance Method

# leakyReLU(with:alphaTensor:name:)

Computes the leaky rectified linear unit (ReLU) activation function on the input tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func leakyReLU(
    with tensor: MPSGraphTensor,
    alphaTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

The operation is: f(x) = max(x, alpha). This operation supports broadcasting with the alpha tensor.

