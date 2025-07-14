

- Metal Performance Shaders Graph
- MPSGraph
-  convolution3D(\_:weights:descriptor:name:) 

Instance Method

# convolution3D(\_:weights:descriptor:name:)

Creates a 3D forward convolution operation and returns the result tensor.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
func convolution3D(
    _ source: MPSGraphTensor,
    weights: MPSGraphTensor,
    descriptor: MPSGraphConvolution3DOpDescriptor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`source`  

Source tensor - must be of rank 5. The layout is defined by `descriptor.dataLayout`.

`weights`  

Weights tensor, must be rank 5. The layout is defined by `descriptor.weightsLayout`.

`descriptor`  

Specifies strides, dilation rates, paddings and layouts.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

