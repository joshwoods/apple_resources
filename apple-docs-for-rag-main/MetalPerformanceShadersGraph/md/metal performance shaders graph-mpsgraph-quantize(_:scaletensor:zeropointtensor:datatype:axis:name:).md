

- Metal Performance Shaders Graph
- MPSGraph
-  quantize(\_:scaleTensor:zeroPointTensor:dataType:axis:name:) 

Instance Method

# quantize(\_:scaleTensor:zeroPointTensor:dataType:axis:name:)

Creates a Quantize operation and returns the result tensor.

iOS 16.2+iPadOS 16.2+Mac Catalyst 16.2+macOS 13.1+tvOS 16.2+visionOS 1.0+

``` source
func quantize(
    _ tensor: MPSGraphTensor,
    scaleTensor: MPSGraphTensor,
    zeroPointTensor: MPSGraphTensor,
    dataType: MPSDataType,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor to be quantized

`scaleTensor`  

Scale scalar or 1D Tensor parameter with size == tensor.shape\[axis\]

`zeroPointTensor`  

Bias scalar or 1D Tensor parameter with size == tensor.shape\[axis\]

`dataType`  

Integer data type of the result tensor.

`axis`  

Axis on which the scale 1D value is being broadcasted

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor array of datatype dataType

## Discussion

Convert the float `tensor` to an i8 or u8 tensor by applying a scale + bias transform: result = (tensor / scaleTensor) + zeroPointTensor

