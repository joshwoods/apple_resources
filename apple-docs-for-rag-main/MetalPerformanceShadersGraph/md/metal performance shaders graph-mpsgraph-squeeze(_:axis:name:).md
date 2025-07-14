

- Metal Performance Shaders Graph
- MPSGraph
-  squeeze(\_:axis:name:) 

Instance Method

# squeeze(\_:axis:name:)

Creates a squeeze operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func squeeze(
    _ tensor: MPSGraphTensor,
    axis: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`axis`  

The axis to squeeze.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Squeezes the tensor, removing a dimension with size 1 at the specified axis. The size of the input tensor must be 1 at the specified axis.

