

- Metal Performance Shaders Graph
- MPSGraph
-  convolutionTranspose2DDataGradient(\_:weights:outputShapeTensor:forwardConvolutionDescriptor:name:) 

Instance Method

# convolutionTranspose2DDataGradient(\_:weights:outputShapeTensor:forwardConvolutionDescriptor:name:)

Creates a convolution transpose gradient operation with respect to the source tensor of convolution transpose operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func convolutionTranspose2DDataGradient(
    _ incomingGradient: MPSGraphTensor,
    weights: MPSGraphTensor,
    outputShapeTensor outputShape: MPSGraphTensor,
    forwardConvolutionDescriptor: MPSGraphConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradient`  

Incoming gradient tensor

`weights`  

Forward pass weights tensor

`outputShape`  

1D Int32 or Int64 Tensor. Shape of the forward pass source tensor

`forwardConvolutionDescriptor`  

Forward pass op descriptor

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Inserts an operation in graph to compute gradient of convolution transpose with respect to source tensor of the corresponding convolution transpose operation.

