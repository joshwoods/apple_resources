

- Metal Performance Shaders Graph
- MPSGraph
-  squeeze(\_:name:) 

Instance Method

# squeeze(\_:name:)

Creates a squeeze operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func squeeze(
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

Squeezes the tensor, removing all dimensions with size 1.

