

- Metal Performance Shaders Graph
- MPSGraph
-  bitwisePopulationCount(\_:name:) 

Instance Method

# bitwisePopulationCount(\_:name:)

Returns the population count of the input tensor elements.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+

``` source
func bitwisePopulationCount(
    _ tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor, which must be of integer type.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

## Discussion

This operation only accepts integer tensors, and returns the number of bits set in the input element.

