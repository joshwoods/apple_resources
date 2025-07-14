

- Metal Performance Shaders Graph
- MPSGraph
-  sliceGradientTensor(\_:fwdInShapeTensor:start:sizeTensor:squeezeMask:name:) 

Instance Method

# sliceGradientTensor(\_:fwdInShapeTensor:start:sizeTensor:squeezeMask:name:)

Creates a slice gradient operation and returns the result tensor.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+

``` source
func sliceGradientTensor(
    _ inputGradientTensor: MPSGraphTensor,
    fwdInShapeTensor: MPSGraphTensor,
    start startTensor: MPSGraphTensor,
    sizeTensor: MPSGraphTensor,
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

`sizeTensor`  

The tensor that specifies the size of the forward result for each dimension.

`squeezeMask`  

A bitmask that indicates dimensions the operation will squeeze out from the result.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

