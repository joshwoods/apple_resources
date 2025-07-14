

- Metal Performance Shaders Graph
- MPSGraph
-  resizeBilinear(withGradientTensor:input:scale:offsetTensor:name:) 

Instance Method

# resizeBilinear(withGradientTensor:input:scale:offsetTensor:name:)

Creates a Resize gradient operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func resizeBilinear(
    withGradientTensor gradient: MPSGraphTensor,
    input: MPSGraphTensor,
    scale: MPSGraphTensor,
    offsetTensor offset: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Incoming gradient tensor

`input`  

Forward pass input tensor

`scale`  

1D float tensor of size equal to rank of input.

`offset`  

1D float tensor of size equal to rank of input.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Computes the gradient for the forward pass Resize op with bilinear sampling and identical parameters.

