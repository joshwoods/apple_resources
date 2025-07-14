

- Metal Performance Shaders Graph
- MPSGraph
-  transpose(\_:permutation:name:) 

Instance Method

# transpose(\_:permutation:name:)

Creates a permutation operation and returns the result tensor.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func transpose(
    _ tensor: MPSGraphTensor,
    permutation: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be permuted.

`permutation`  

An array of numbers defining the permutation, must be of length `rank(tensor)` and define a valid permutation.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Permutes the dimensions of the input tensor according to values in `permutation`.

