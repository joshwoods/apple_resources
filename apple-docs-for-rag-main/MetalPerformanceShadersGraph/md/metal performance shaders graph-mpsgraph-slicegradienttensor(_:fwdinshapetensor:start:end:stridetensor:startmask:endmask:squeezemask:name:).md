

- Metal Performance Shaders Graph
- MPSGraph
-  sliceGradientTensor(\_:fwdInShapeTensor:start:end:strideTensor:startMask:endMask:squeezeMask:name:) 

Instance Method

# sliceGradientTensor(\_:fwdInShapeTensor:start:end:strideTensor:startMask:endMask:squeezeMask:name:)

Creates a strided-slice gradient operation and returns the result tensor.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+

``` source
func sliceGradientTensor(
    _ inputGradientTensor: MPSGraphTensor,
    fwdInShapeTensor: MPSGraphTensor,
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

`inputGradientTensor`  

The input gradient.

`fwdInShapeTensor`  

The shape of the forward pass input, that is the shape of the gradient output.

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

A valid MPSGraphTensor object

