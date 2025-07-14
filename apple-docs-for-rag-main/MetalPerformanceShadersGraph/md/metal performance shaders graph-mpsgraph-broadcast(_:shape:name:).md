

- Metal Performance Shaders Graph
- MPSGraph
-  broadcast(\_:shape:name:) 

Instance Method

# broadcast(\_:shape:name:)

Creates a broadcast operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func broadcast(
    _ tensor: MPSGraphTensor,
    shape: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be broadcasted

`shape`  

The shape of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Broadcasts values inside the tensor, starting from the trailing dimensions, to give it the correct shape. This is equivalent to the broadcasting for arithmetic operations when operands have different shapes.

