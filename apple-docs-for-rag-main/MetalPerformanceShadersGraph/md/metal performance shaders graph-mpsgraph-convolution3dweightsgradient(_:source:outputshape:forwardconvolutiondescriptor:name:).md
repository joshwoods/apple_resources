

- Metal Performance Shaders Graph
- MPSGraph
-  convolution3DWeightsGradient(\_:source:outputShape:forwardConvolutionDescriptor:name:) 

Instance Method

# convolution3DWeightsGradient(\_:source:outputShape:forwardConvolutionDescriptor:name:)

Creates a 3D convolution gradient operation with respect to the weights tensor of the forward convolution.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
func convolution3DWeightsGradient(
    _ incomingGradient: MPSGraphTensor,
    source: MPSGraphTensor,
    outputShape: [NSNumber],
    forwardConvolutionDescriptor: MPSGraphConvolution3DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradient`  

Incoming loss gradient tensor

`outputShape`  

Shape of the forward pass source tensor

`forwardConvolutionDescriptor`  

Forward convolution 2D op `descriptor`

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

If `W` is weights tensor to forward convolution, `R` is the result/returned tensor of forward convolution, and `L` is the loss function, convolution3DWeightsGradientWithIncomingGradientTensor returns tensor `dL/dW = dL/dR * dR/dW`, where `dL/dR` is the incomingGradient parameter.

