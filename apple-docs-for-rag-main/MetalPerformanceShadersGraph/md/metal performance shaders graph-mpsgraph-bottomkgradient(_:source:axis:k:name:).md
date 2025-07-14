

- Metal Performance Shaders Graph
- MPSGraph
-  bottomKGradient(\_:source:axis:k:name:) 

Instance Method

# bottomKGradient(\_:source:axis:k:name:)

Creates a BottomKGradient operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func bottomKGradient(
    _ gradient: MPSGraphTensor,
    source: MPSGraphTensor,
    axis: Int,
    k: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`gradient`  

Tensor containing the incoming gradient.

`source`  

Tensor containing source data.

`axis`  

The dimension along which to compute the BottomK values.

`k`  

The number of largest values to return.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Finds the K smallest values along the minor dimension of the input. The input must have at least K elements along its minor dimension.

