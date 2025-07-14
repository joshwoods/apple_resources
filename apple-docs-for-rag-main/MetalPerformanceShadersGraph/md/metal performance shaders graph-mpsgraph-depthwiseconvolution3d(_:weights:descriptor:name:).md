

- Metal Performance Shaders Graph
- MPSGraph
-  depthwiseConvolution3D(\_:weights:descriptor:name:) 

Instance Method

# depthwiseConvolution3D(\_:weights:descriptor:name:)

Creates a 3D depthwise convolution operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func depthwiseConvolution3D(
    _ source: MPSGraphTensor,
    weights: MPSGraphTensor,
    descriptor: MPSGraphDepthwiseConvolution3DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

A 3D Image source as tensor - must be at least rank=4 (CDHW when channelDimensionIndex = -4).

`weights`  

The weights tensor, must be rank=4 - axes are interpreted as CDHW when channelDimensionIndex = -4 .

`descriptor`  

The descriptor object that specifies strides, dilation rates and paddings.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Works exactly like depthwise convolution2D, but in three dimensions. Supports different layouts with the channelDimensionIndex property. If your weights need a different layout add a permute operation on them before this operation.

