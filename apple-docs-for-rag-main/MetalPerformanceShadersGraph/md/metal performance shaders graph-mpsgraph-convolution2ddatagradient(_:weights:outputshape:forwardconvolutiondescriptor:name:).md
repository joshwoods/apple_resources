

- Metal Performance Shaders Graph
- MPSGraph
-  convolution2DDataGradient(\_:weights:outputShape:forwardConvolutionDescriptor:name:) 

Instance Method

# convolution2DDataGradient(\_:weights:outputShape:forwardConvolutionDescriptor:name:)

Creates a 2D convolution gradient operation with respect to the source tensor of the forward convolution.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func convolution2DDataGradient(
    _ incomingGradient: MPSGraphTensor,
    weights: MPSGraphTensor,
    outputShape: [NSNumber],
    forwardConvolutionDescriptor: MPSGraphConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradient`  

Incoming loss gradient tensor

`weights`  

Forward pass weights tensor

`outputShape`  

Shape of the forward pass source tensor

`forwardConvolutionDescriptor`  

Forward convolution 2D op `descriptor`

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

If `S` is source tensor to forward convolution, `R` is the result/returned tensor from forward convolution, and `L` is the loss function, `convolution2DDataGradientWithIncomingGradientTensor` returns tensor `dL/dS = dL/dR * dR/dS`, where `dL/dR` is the incomingGradient parameter.

