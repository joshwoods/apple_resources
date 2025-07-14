

- Metal Performance Shaders Graph
- MPSGraph
-  variance(of:axes:name:) 

Instance Method

# variance(of:axes:name:)

Returns the variance of the first input along the specified axes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func variance(
    of tensor: MPSGraphTensor,
    axes: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axes`  

A list of axes over which to perform the reduction. Tthe order of dimensions goes from the slowest moving at axis=0 to the fastest moving dimension.

`name`  

An optional name for the operation.

## Return Value

A valid `MPSGraphTensor` object.

