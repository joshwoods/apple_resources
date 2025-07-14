

- Metal Performance Shaders Graph
- MPSGraph
-  reverse(\_:name:) 

Instance Method

# reverse(\_:name:)

Creates a reverse operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func reverse(
    _ tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be reversed.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Reverses a tensor on all axes. Semantics based on TensorFlow reverse op.

