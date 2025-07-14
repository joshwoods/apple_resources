

- Metal Performance Shaders Graph
- MPSGraph
-  depthwiseConvolution2DDataGradient(\_:weights:outputShape:descriptor:name:) 

Instance Method

# depthwiseConvolution2DDataGradient(\_:weights:outputShape:descriptor:name:)

Creates a 2D-depthwise convolution gradient for data operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func depthwiseConvolution2DDataGradient(
    _ incomingGradient: MPSGraphTensor,
    weights: MPSGraphTensor,
    outputShape: [NSNumber],
    descriptor: MPSGraphDepthwiseConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradient`  

A 2D input gradient tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`weights`  

The weights tensor, must be rank=4. The layout is defined by `descriptor.weightsLayout`.

`outputShape`  

The shape of the οutput tensor (and therefore input tensor of forward pass).

`descriptor`  

The descriptor object that specifies strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

