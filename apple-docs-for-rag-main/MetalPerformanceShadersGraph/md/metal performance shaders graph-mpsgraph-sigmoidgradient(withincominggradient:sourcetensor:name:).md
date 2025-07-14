

- Metal Performance Shaders Graph
- MPSGraph
-  sigmoidGradient(withIncomingGradient:sourceTensor:name:) 

Instance Method

# sigmoidGradient(withIncomingGradient:sourceTensor:name:)

Computes the gradient of the sigmoid function using the incoming gradient tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func sigmoidGradient(
    withIncomingGradient gradient: MPSGraphTensor,
    sourceTensor source: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

The incoming gradient tensor.

`source`  

The input tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

