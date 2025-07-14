

- Metal Performance Shaders Graph
- MPSGraph
-  quantize(\_:scale:zeroPoint:dataType:name:) 

Instance Method

# quantize(\_:scale:zeroPoint:dataType:name:)

Creates a Quantize operation and returns the result tensor.

iOS 16.2+iPadOS 16.2+Mac Catalyst 16.2+macOS 13.1+tvOS 16.2+visionOS 1.0+

``` source
func quantize(
    _ tensor: MPSGraphTensor,
    scale: Double,
    zeroPoint: Double,
    dataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor to be quantized

`scale`  

Scale scalar parameter

`zeroPoint`  

Bias scalar parameter (converted to dataType of resultTensor)

`dataType`  

Integer data type of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor array of datatype dataType

## Discussion

Convert the float `tensor` to an i8 or u8 tensor by applying a scale + bias transform: result = (tensor / scale) + zeroPoint

