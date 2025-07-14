

- Metal Performance Shaders Graph
- MPSGraph
-  depthwiseConvolution2DWeightsGradient(\_:source:outputShape:descriptor:name:) 

Instance Method

# depthwiseConvolution2DWeightsGradient(\_:source:outputShape:descriptor:name:)

Creates a 2D-depthwise convolution gradient for weights operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func depthwiseConvolution2DWeightsGradient(
    _ incomingGradient: MPSGraphTensor,
    source: MPSGraphTensor,
    outputShape: [NSNumber],
    descriptor: MPSGraphDepthwiseConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`incomingGradient`  

A 2D input gradient tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`source`  

A 2D Image source as tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`outputShape`  

The shape of the οutput tensor (and therefore weight tensor of forward pass).

`descriptor`  

The descriptor object that specifies strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

