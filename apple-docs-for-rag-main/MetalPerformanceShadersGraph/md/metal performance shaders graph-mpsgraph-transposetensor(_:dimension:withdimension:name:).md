

- Metal Performance Shaders Graph
- MPSGraph
-  transposeTensor(\_:dimension:withDimension:name:) 

Instance Method

# transposeTensor(\_:dimension:withDimension:name:)

Creates a transpose operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func transposeTensor(
    _ tensor: MPSGraphTensor,
    dimension dimensionIndex: Int,
    withDimension dimensionIndex2: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be transposed.

`dimensionIndex`  

The first dimension index to be transposed.

`dimensionIndex2`  

The second dimension index to be transposed.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Transposes the dimensions `dimensionIndex` and `dimensionIndex2` of the input tensor.

