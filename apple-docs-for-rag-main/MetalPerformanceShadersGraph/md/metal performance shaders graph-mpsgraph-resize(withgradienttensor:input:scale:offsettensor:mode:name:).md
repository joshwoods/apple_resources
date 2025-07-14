

- Metal Performance Shaders Graph
- MPSGraph
-  resize(withGradientTensor:input:scale:offsetTensor:mode:name:) 

Instance Method

# resize(withGradientTensor:input:scale:offsetTensor:mode:name:)

Creates a Resize gradient operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func resize(
    withGradientTensor gradient: MPSGraphTensor,
    input: MPSGraphTensor,
    scale: MPSGraphTensor,
    offsetTensor offset: MPSGraphTensor,
    mode: MPSGraphResizeMode,
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

`mode`  

The resampling mode to use. If nearest sampling is specifed, RoundPreferCeil mode will be used.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Computes the gradient for the forward pass Resize op with identical parameters. See discussion of resizeTensor for more in depth description of resize paramters.

