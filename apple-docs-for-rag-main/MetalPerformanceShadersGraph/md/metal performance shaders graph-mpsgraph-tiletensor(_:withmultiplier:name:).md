

- Metal Performance Shaders Graph
- MPSGraph
-  tileTensor(\_:withMultiplier:name:) 

Instance Method

# tileTensor(\_:withMultiplier:name:)

Creates a tile operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func tileTensor(
    _ tensor: MPSGraphTensor,
    withMultiplier multiplier: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor

`multiplier`  

An array of numbers that specifies how many copies per dimension MPSGraph produces.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Creates a tensor which contains multiple copies of the input tensor along each dimension of the tensor.

