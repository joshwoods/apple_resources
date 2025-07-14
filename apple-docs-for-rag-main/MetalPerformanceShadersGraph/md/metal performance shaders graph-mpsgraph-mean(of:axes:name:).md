

- Metal Performance Shaders Graph
- MPSGraph
-  mean(of:axes:name:) 

Instance Method

# mean(of:axes:name:)

Returns the mean of the first input along the specified axes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func mean(
    of tensor: MPSGraphTensor,
    axes: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axes`  

A list of axes over which to perform the reduction. The order of dimensions goes from the slowest moving at axis=0 to the fastest moving dimension.

`name`  

An optional name for the operation.

## Return Value

A valid `MPSGraphTensor` object.

