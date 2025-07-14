

- Metal Performance Shaders Graph
- MPSGraph
-  shapeOf(\_:name:) 

Instance Method

# shapeOf(\_:name:)

Creates a shape-of operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func shapeOf(
    _ tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Returns a rank-1 tensor of type `MPSDataTypeInt32` with the values of the static shape of the input tensor.

