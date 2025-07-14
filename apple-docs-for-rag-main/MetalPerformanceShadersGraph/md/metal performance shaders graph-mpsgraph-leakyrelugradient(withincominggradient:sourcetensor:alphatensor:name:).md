

- Metal Performance Shaders Graph
- MPSGraph
-  leakyReLUGradient(withIncomingGradient:sourceTensor:alphaTensor:name:) 

Instance Method

# leakyReLUGradient(withIncomingGradient:sourceTensor:alphaTensor:name:)

Computes the gradient of the leaky rectified linear unit (ReLU) activation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func leakyReLUGradient(
    withIncomingGradient gradient: MPSGraphTensor,
    sourceTensor source: MPSGraphTensor,
    alphaTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

The incoming gradient tensor.

`source`  

The input tensor in forward pass.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

This operation supports broadcasting with the alpha tensor.

