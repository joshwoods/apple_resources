

- Metal Performance Shaders Graph
- MPSGraph
-  softMaxGradient(withIncomingGradient:sourceTensor:axis:name:) 

Instance Method

# softMaxGradient(withIncomingGradient:sourceTensor:axis:name:)

Computes the gradient of the softmax function along the specified axis using the incoming gradient tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func softMaxGradient(
    withIncomingGradient gradient: MPSGraphTensor,
    sourceTensor source: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

The incoming gradient tensor.

`source`  

The input tensor.

`axis`  

The axis along which softmax is computed.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

