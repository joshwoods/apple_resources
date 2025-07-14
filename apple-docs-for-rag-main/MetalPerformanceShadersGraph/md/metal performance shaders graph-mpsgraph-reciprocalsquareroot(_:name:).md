

- Metal Performance Shaders Graph
- MPSGraph
-  reciprocalSquareRoot(\_:name:) 

Instance Method

# reciprocalSquareRoot(\_:name:)

Applies the reciprocal square root operation to the input tensor elements.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func reciprocalSquareRoot(
    _ tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

