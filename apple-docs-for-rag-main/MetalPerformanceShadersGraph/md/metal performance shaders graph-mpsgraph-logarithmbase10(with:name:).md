

- Metal Performance Shaders Graph
- MPSGraph
-  logarithmBase10(with:name:) 

Instance Method

# logarithmBase10(with:name:)

Computes the logarithm with base 10 to the input tensor elements.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func logarithmBase10(
    with tensor: MPSGraphTensor,
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

