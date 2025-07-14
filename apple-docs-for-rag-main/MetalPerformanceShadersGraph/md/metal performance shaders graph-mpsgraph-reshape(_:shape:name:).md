

- Metal Performance Shaders Graph
- MPSGraph
-  reshape(\_:shape:name:) 

Instance Method

# reshape(\_:shape:name:)

Creates a reshape operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func reshape(
    _ tensor: MPSGraphTensor,
    shape: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be reshaped.

`shape`  

The result tensor shape.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

This operation reshapes the input tensor to the target shape. The shape must be compatible with the input tensor shape, specifically the volume of the input tensor has to match the volume defined by the shape. The shape is allowed to contain dynamic dimensions (-1) when the result type can be inferred unambiguously.

