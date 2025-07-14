

- Metal Performance Shaders Graph
- MPSGraph
-  sliceUpdateDataTensor(\_:update:starts:ends:strides:startMask:endMask:squeezeMask:name:) 

Instance Method

# sliceUpdateDataTensor(\_:update:starts:ends:strides:startMask:endMask:squeezeMask:name:)

Creates a strided-slice update operation and returns the result tensor.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
func sliceUpdateDataTensor(
    _ dataTensor: MPSGraphTensor,
    update updateTensor: MPSGraphTensor,
    starts: [NSNumber],
    ends: [NSNumber],
    strides: [NSNumber],
    startMask: UInt32,
    endMask: UInt32,
    squeezeMask: UInt32,
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

`startMask`  

A bitmask that indicates dimensions whose `starts` values the operation should ignore.

`endMask`  

A bitmask that indicates dimensions whose `ends` values the operation should ignore.

`squeezeMask`  

A bitmask that indicates dimensions the operation will squeeze out from the result.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

