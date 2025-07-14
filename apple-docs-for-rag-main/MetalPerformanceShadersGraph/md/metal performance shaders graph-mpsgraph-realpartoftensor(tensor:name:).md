

- Metal Performance Shaders Graph
- MPSGraph
-  realPartOfTensor(tensor:name:) 

Instance Method

# realPartOfTensor(tensor:name:)

Returns the real part of a tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func realPartOfTensor(
    tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

An optional string which serves as an identifier for the operation..

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

