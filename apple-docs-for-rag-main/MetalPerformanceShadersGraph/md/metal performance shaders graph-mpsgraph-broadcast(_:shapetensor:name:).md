

- Metal Performance Shaders Graph
- MPSGraph
-  broadcast(\_:shapeTensor:name:) 

Instance Method

# broadcast(\_:shapeTensor:name:)

Creates a broadcast operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func broadcast(
    _ tensor: MPSGraphTensor,
    shapeTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The Tensor to be broadcasted.

`shapeTensor`  

A rank-1 tensor of type `MPSDataTypeInt32` or `MPSDataTypeInt64` that defines the shape of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Broadcasts values inside the tensor, starting from the trailing dimensions, to give it the correct shape. This is equivalent to the broadcasting for arithmetic operations when operands have different shapes.

