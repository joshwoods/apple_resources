

- Metal Performance Shaders Graph
- MPSGraph
-  expandDims(\_:axesTensor:name:) 

Instance Method

# expandDims(\_:axesTensor:name:)

Creates an expand-dimensions operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func expandDims(
    _ tensor: MPSGraphTensor,
    axesTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`axesTensor`  

The tensor containing the axes to expand.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Expands the tensor, inserting dimensions with size 1 at specified axes.

