

- Metal Performance Shaders Graph
- MPSGraph
-  sliceUpdateDataTensor(\_:update:starts:ends:strides:name:) 

Instance Method

# sliceUpdateDataTensor(\_:update:starts:ends:strides:name:)

Creates a strided-slice update operation with zero masks and returns the result tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func sliceUpdateDataTensor(
    _ dataTensor: MPSGraphTensor,
    update updateTensor: MPSGraphTensor,
    starts: [NSNumber],
    ends: [NSNumber],
    strides: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`dataTensor`  

The large tensor that will receive the update.

`updateTensor`  

The tensor with the new values that will replace values in the dataTensor.

`starts`  

An array of numbers that specify the starting points for each dimension.

`ends`  

An array of numbers that specify the ending points for each dimension.

`strides`  

An array of numbers that specify the strides for each dimension.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

