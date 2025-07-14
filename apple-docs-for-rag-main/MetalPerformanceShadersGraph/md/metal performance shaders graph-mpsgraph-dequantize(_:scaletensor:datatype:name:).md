

- Metal Performance Shaders Graph
- MPSGraph
-  dequantize(\_:scaleTensor:dataType:name:) 

Instance Method

# dequantize(\_:scaleTensor:dataType:name:)

Creates a dequantize operation and returns the result tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func dequantize(
    _ tensor: MPSGraphTensor,
    scaleTensor: MPSGraphTensor,
    dataType: MPSDataType,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor to be dequantized.

`scaleTensor`  

Scale Tensor parameter with groups support.

`dataType`  

Float data type of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor array of datatype `dataType`.

## Discussion

Converts the i8, u8, i4 or u4 `tensor` to a float tensor by applying a scale and bias transform:

```
result = scaleTensor * tensor.
```

