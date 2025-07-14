

- Metal Performance Shaders Graph
- MPSGraph
-  dropout(\_:rate:name:) 

Instance Method

# dropout(\_:rate:name:)

Creates a dropout operation and returns the result

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func dropout(
    _ tensor: MPSGraphTensor,
    rate: Double,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

Input tensor

`rate`  

The rate of values to be set to 0

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object

## Discussion

Removes values in the `tensor` with a percentage chance equal to `rate`. Removed values are set to 0

