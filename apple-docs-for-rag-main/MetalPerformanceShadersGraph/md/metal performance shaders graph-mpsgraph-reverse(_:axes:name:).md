

- Metal Performance Shaders Graph
- MPSGraph
-  reverse(\_:axes:name:) 

Instance Method

# reverse(\_:axes:name:)

Creates a reverse operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func reverse(
    _ tensor: MPSGraphTensor,
    axes: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be reversed.

`axes`  

A tensor that specifies axes to be reversed (Axes must be unique and within normal axis range).

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Reverses a tensor on given axes. Semantics based on TensorFlow reverse op.

