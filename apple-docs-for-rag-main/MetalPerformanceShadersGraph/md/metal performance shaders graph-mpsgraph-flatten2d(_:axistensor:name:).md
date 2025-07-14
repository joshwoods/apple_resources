

- Metal Performance Shaders Graph
- MPSGraph
-  flatten2D(\_:axisTensor:name:) 

Instance Method

# flatten2D(\_:axisTensor:name:)

Creates a flatten2D operation and returns the result tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func flatten2D(
    _ tensor: MPSGraphTensor,
    axisTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be flattened.

`axisTensor`  

A scalar tensor that contains the axis around which to flatten.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Flattens dimensions before `axis` to `result[0]` and dimensions starting from `axis` to `result[1]` and returns a rank-2 tensor as result.

