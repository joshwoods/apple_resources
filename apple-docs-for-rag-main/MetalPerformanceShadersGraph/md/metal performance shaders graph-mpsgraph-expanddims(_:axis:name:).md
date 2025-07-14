

- Metal Performance Shaders Graph
- MPSGraph
-  expandDims(\_:axis:name:) 

Instance Method

# expandDims(\_:axis:name:)

Creates an expand-dimensions operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func expandDims(
    _ tensor: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`axis`  

The axis to expand.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Expands the tensor, inserting a dimension with size 1 at the specified axis.

