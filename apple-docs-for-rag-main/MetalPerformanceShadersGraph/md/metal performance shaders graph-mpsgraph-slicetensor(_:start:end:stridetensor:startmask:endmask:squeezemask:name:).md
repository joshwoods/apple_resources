

- Metal Performance Shaders Graph
- MPSGraph
-  sliceTensor(\_:start:end:strideTensor:startMask:endMask:squeezeMask:name:) 

Instance Method

# sliceTensor(\_:start:end:strideTensor:startMask:endMask:squeezeMask:name:)

Creates a strided-slice operation and returns the result tensor.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+

``` source
func sliceTensor(
    _ tensor: MPSGraphTensor,
    start startTensor: MPSGraphTensor,
    end endTensor: MPSGraphTensor,
    strideTensor: MPSGraphTensor,
    startMask: UInt32,
    endMask: UInt32,
    squeezeMask: UInt32,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The Tensor to be sliced.

`startTensor`  

The tensor that specifies the starting points for each dimension.

`endTensor`  

The tensor that specifies the ending points for each dimension.

`strideTensor`  

The tensor that specifies the strides for each dimension.

`startMask`  

A bitmask that indicates dimensions whose `starts` values the operation should ignore.

`endMask`  

A bitmask that indicates dimensions whose `ends` values the operation should ignore.

`squeezeMask`  

A bitmask that indicates dimensions the operation will squeeze out from the result.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Slices a tensor starting from `startTensor`, stopping short before `endTensor` stepping `strideTensor` paces between each value. Semantics based on TensorFlow Strided Slice Op.

