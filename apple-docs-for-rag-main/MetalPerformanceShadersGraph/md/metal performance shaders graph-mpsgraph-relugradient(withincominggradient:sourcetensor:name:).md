

- Metal Performance Shaders Graph
- MPSGraph
-  reLUGradient(withIncomingGradient:sourceTensor:name:) 

Instance Method

# reLUGradient(withIncomingGradient:sourceTensor:name:)

Computes the gradient of the ReLU (rectified linear activation unit) function using the incoming gradient.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func reLUGradient(
    withIncomingGradient gradient: MPSGraphTensor,
    sourceTensor source: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

The incoming gradient tensor.

`source`  

The input tensor from forward pass.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

