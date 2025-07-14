

- Metal Performance Shaders Graph
- MPSGraph
-  depthwiseConvolution2D(\_:weights:descriptor:name:) 

Instance Method

# depthwiseConvolution2D(\_:weights:descriptor:name:)

Creates a 2D-depthwise convolution operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func depthwiseConvolution2D(
    _ source: MPSGraphTensor,
    weights: MPSGraphTensor,
    descriptor: MPSGraphDepthwiseConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

A 2D Image source as tensor - must be of rank=4. The layout is defined by `descriptor.dataLayout`.

`weights`  

The weights tensor, must be rank=4. The layout is defined by `descriptor.weightsLayout`.

`descriptor`  

The descriptor object that specifies strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

