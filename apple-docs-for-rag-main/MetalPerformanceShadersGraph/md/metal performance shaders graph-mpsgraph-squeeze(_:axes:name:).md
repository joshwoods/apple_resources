

- Metal Performance Shaders Graph
- MPSGraph
-  squeeze(\_:axes:name:) 

Instance Method

# squeeze(\_:axes:name:)

Creates a squeeze operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func squeeze(
    _ tensor: MPSGraphTensor,
    axes: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`axes`  

The axes to squeeze.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Squeezes the tensor, removing dimensions with size 1 at specified axes. The size of the input tensor must be 1 at all specified axes.

