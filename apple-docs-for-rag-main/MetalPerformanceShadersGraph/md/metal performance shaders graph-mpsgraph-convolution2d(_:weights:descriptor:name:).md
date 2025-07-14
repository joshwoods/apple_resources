

- Metal Performance Shaders Graph
- MPSGraph
-  convolution2D(\_:weights:descriptor:name:) 

Instance Method

# convolution2D(\_:weights:descriptor:name:)

Creates a 2D (forward) convolution operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func convolution2D(
    _ source: MPSGraphTensor,
    weights: MPSGraphTensor,
    descriptor: MPSGraphConvolution2DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

Source tensor - must be a rank 4 tensor. The layout is defined by `descriptor.dataLayout`.

`weights`  

Weights tensor, must be rank 4. The layout is defined by `descriptor.weightsLayout`.

`descriptor`  

Specifies strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

