

- Metal Performance Shaders Graph
- MPSGraph
-  convolution2DWeightsGradient(\_:source:outputShape:forwardConvolutionDescriptor:name:) 

Instance Method

# convolution2DWeightsGradient(\_:source:outputShape:forwardConvolutionDescriptor:name:)

Creates a 2D convolution gradient operation with respect to the weights tensor of the forward convolution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func convolution2DWeightsGradient(
    _ incomingGradient: MPSGraphTensor,
    source: MPSGraphTensor,
    outputShape: [NSNumber],
    forwardConvolutionDescriptor: MPSGraphConvolution2DOpDescriptor,
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

If `W` is weights tensor to forward convolution, `R` is the result/returned tensor of forward convolution, and `L` is the loss function, convolution2DWeightsGradientWithIncomingGradientTensor returns tensor `dL/dW = dL/dR * dR/dW`, where `dL/dR` is the incomingGradient parameter.

