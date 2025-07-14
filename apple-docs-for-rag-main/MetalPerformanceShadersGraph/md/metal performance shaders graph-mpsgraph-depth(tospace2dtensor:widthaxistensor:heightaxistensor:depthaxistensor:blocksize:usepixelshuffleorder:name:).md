

- Metal Performance Shaders Graph
- MPSGraph
-  depth(toSpace2DTensor:widthAxisTensor:heightAxisTensor:depthAxisTensor:blockSize:usePixelShuffleOrder:name:) 

Instance Method

# depth(toSpace2DTensor:widthAxisTensor:heightAxisTensor:depthAxisTensor:blockSize:usePixelShuffleOrder:name:)

Creates a depth-to-space2D operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func depth(
    toSpace2DTensor tensor: MPSGraphTensor,
    widthAxisTensor: MPSGraphTensor,
    heightAxisTensor: MPSGraphTensor,
    depthAxisTensor: MPSGraphTensor,
    blockSize: Int,
    usePixelShuffleOrder: Bool,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`widthAxisTensor`  

A scalar tensor that contains the axis that defines the fastest running dimension within the block.

`heightAxisTensor`  

A scalar tensor that contains the axis that defines the 2nd fastest running dimension within the block.

`depthAxisTensor`  

A scalar tensor that contains the axis that defines the destination dimension, where to copy the blocks.

`blockSize`  

The size of the square spatial sub-block.

`usePixelShuffleOrder`  

A parameter that controls the layout of the sub-blocks within the depth dimension.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

This operation outputs a copy of the input tensor, where values from the `depthAxisTensor` dimension are moved in spatial blocks of size `blockSize` to the `heightAxisTensor` and `widthAxisTensor` dimensions. Use the `usePixelShuffleOrder` parameter to control how the data within spatial blocks is ordered in the `depthAxisTensor` dimension: with `usePixelShuffleOrder = YES` MPSGraph stores the values of the spatial block contiguosly within the `depthAxisTensor` dimension, whereas without it they are stored interleaved with existing values in the `depthAxisTensor` dimension. This operation is the inverse of space(toDepth2DTensor:widthAxisTensor:heightAxisTensor:depthAxisTensor:blockSize:usePixelShuffleOrder:name:).

