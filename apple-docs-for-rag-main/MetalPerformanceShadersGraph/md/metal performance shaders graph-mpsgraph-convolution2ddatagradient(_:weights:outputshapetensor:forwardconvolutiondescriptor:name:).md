

- Metal Performance Shaders Graph
- MPSGraph
-  convolution2DDataGradient(\_:weights:outputShapeTensor:forwardConvolutionDescriptor:name:) 

Instance Method

# convolution2DDataGradient(\_:weights:outputShapeTensor:forwardConvolutionDescriptor:name:)

Creates a 2D convolution gradient operation with respect to the source tensor of the forward convolution.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func convolution2DDataGradient(
    _ gradient: MPSGraphTensor,
    weights: MPSGraphTensor,
    outputShapeTensor: MPSGraphTensor,
    forwardConvolutionDescriptor: MPSGraphConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`weights`  

Forward pass weights tensor

`outputShapeTensor`  

4D Int32 or Int64 tensor. Shape of the forward pass source tensor

`forwardConvolutionDescriptor`  

Forward convolution 2D op `descriptor`

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

If `S` is source tensor to forward convolution, `R` is the result/returned tensor of forward convolution, and `L` is the loss function, convolution2DDataGradientWithIncomingGradientTensor returns tensor `dL/dS = dL/dR * dR/dS`, where `dL/dR` is the incomingGradient parameter.

